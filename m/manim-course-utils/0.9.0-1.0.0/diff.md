# Comparing `tmp/manim_course_utils-0.9.0.tar.gz` & `tmp/manim_course_utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_course_utils-0.9.0.tar", max compression
+gzip compressed data, was "manim_course_utils-1.0.0.tar", max compression
```

## Comparing `manim_course_utils-0.9.0.tar` & `manim_course_utils-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      112 2023-05-11 22:31:16.319862 manim_course_utils-0.9.0/manim_course_utils/__init__.py
--rw-r--r--   0        0        0     2971 2023-05-18 15:00:51.357510 manim_course_utils-0.9.0/manim_course_utils/animation_description.py
--rw-r--r--   0        0        0      318 2023-05-18 15:11:19.800699 manim_course_utils-0.9.0/manim_course_utils/markdown_tex_template.py
--rw-r--r--   0        0        0     2082 2023-05-18 15:00:22.904911 manim_course_utils-0.9.0/manim_course_utils/mobject_description.py
--rw-r--r--   0        0        0      520 2023-05-18 15:11:29.768456 manim_course_utils-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      168 2023-05-11 16:15:04.015818 manim_course_utils-0.9.0/README.md
--rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 manim_course_utils-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      111 2023-05-20 02:02:06.855754 manim_course_utils-1.0.0/manim_course_utils/__init__.py
+-rw-r--r--   0        0        0     2174 2023-05-20 21:50:13.928681 manim_course_utils-1.0.0/manim_course_utils/animation_description.py
+-rw-r--r--   0        0        0     1816 2023-05-20 21:51:34.659193 manim_course_utils-1.0.0/manim_course_utils/mobject_description.py
+-rw-r--r--   0        0        0     1570 2023-05-20 21:41:11.763548 manim_course_utils-1.0.0/manim_course_utils/rst_mobject.py
+-rw-r--r--   0        0        0      579 2023-05-20 21:52:30.503656 manim_course_utils-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-11 16:15:04.015818 manim_course_utils-1.0.0/README.md
+-rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 manim_course_utils-1.0.0/PKG-INFO
```

### Comparing `manim_course_utils-0.9.0/manim_course_utils/animation_description.py` & `manim_course_utils-1.0.0/manim_course_utils/animation_description.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,54 @@
 from manim import *
-from manim_course_utils.markdown_tex_template import MarkdownTexTemplate
+from .rst_mobject import RstMobject
 
 
 __all__ = ["AnimationDescription"]
 
 
 class AnimationDescription(Group):
     def __init__(
         self,
         mobject_to_animate: Mobject,
         animation: Animation,
         title: str | None = None,
         description: str | None = None,
-        rec_config: dict | None = None
+        rec_config: dict | None = None,
+        height: float | None = None,
+        buff: float = None,
+        **kwargs
     ):
-        super().__init__()
+        super().__init__(**kwargs)
         self.mobject_to_animate = mobject_to_animate
         self.animation = animation
-        self.title = animation.__class__.__name__ or title
-        self.description = description or animation.__doc__
+        self.title = animation.__class__.__name__ if title is None else title
+        self.description = animation.__doc__ if description is None else description
         examples_idx = self.description.find("Examples")
         if examples_idx != -1:
             self.description = self.description[:examples_idx]
-        self.rec_config = rec_config or {
+        self.description = self.description.split("\n")
+        for i in range(1, len(self.description)):
+            self.description[i] = self.description[i].removeprefix(4 * " ")
+        self.description = "\n".join(self.description)
+        self.description.replace("~.", "")
+        self.rec_config = {
             "stroke_color": WHITE,
             "stroke_width": 2,
             "fill_color": BLACK,
             "fill_opacity": 0.5,
             "buff": 0.2,
             "corner_radius": 0.2
-        }
-        self.title_mobject = Tex(f"\\textbf{{{self.title}}}", font_size=36)
-        self.description_mobject = Tex(self.description, font_size=24, tex_environment="markdown", tex_template=MarkdownTexTemplate())
+        } if rec_config is None else rec_config
+        self.title_mobject = Tex(f"\\textbf{{{self.title}}}")
+        self.description_mobject = RstMobject(self.description).scale_to_fit_height(5)
         self.add(self.title_mobject, self.mobject_to_animate, self.description_mobject)
-        self.arrange(DOWN, buff=0.5)
-        self.add(SurroundingRectangle(self, **self.rec_config))
-    
-    def set_description(self, description: str):
-        self.description = description
-        self[2].become(Tex(self.description, font_size=24, tex_environment="markdown", tex_template=MarkdownTexTemplate()))
-        return self
-    
-    def set_title(self, title: str):
-        self.title = title
-        self[0].become(Tex(f"\\textbf{{{title}}}", font_size=36))
-        return self
-    
-    def set_mobject_and_animation(
-        self,
-        mobject_to_animate: Mobject,
-        animation: Animation,
-        description: str | None = None,
-        title: str | None = None
-    ):
-        self[1].become(mobject_to_animate)
-        self.set_description(description or animation.__doc__)
-        self.set_title(animation.__class__.__name__ or title)
-        self.animation = animation
-        return self
-    
-    def set_animation(self, animation: Animation, description: str | None = None, title: str | None = None):
-        self.set_mobject_and_animation(self.mobject_to_animate, animation, description, title)
-        return self
-    
-    def set_mobject(self, mobject: Mobject, description: str | None = None, title: str | None = None):
-        self.set_mobject_and_animation(mobject, self.animation, description, title)
-        return self
-    
+        buff = 0.5 if buff is None else buff
+        self.arrange(DOWN, buff=buff)
+        self.add_to_back(SurroundingRectangle(self, **self.rec_config))
+        height = 7 if height is None else height
+        self.scale_to_fit_height(height)
+
     def play_animation(self, scene: Scene, run_time: float | None = 1, **kwargs):
         if run_time is not None:
             kwargs["run_time"] = run_time
         scene.play(self.animation, **kwargs)
         return self
```

### Comparing `manim_course_utils-0.9.0/manim_course_utils/mobject_description.py` & `manim_course_utils-1.0.0/manim_course_utils/mobject_description.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,46 @@
 from manim import *
-from manim_course_utils.markdown_tex_template import MarkdownTexTemplate
+from .rst_mobject import RstMobject
 
 
 __all__ = ["MobjectDescription"]
 
 
 class MobjectDescription(Group):
     def __init__(
         self,
         mobject: Mobject,
         title: str | None = None,
         description: str | None = None,
         rec_config: dict | None = None,
+        height: float | None = None,
+        buff: float = None,
         **kwargs
     ):
         super().__init__(**kwargs)
         self.mobject = mobject
         self.description = mobject.__doc__ if description is None else description
         examples_idx = self.description.find("Examples")
         if examples_idx != -1:
             self.description = self.description[:examples_idx]
-        self.title = mobject.__class__.__name__ or title
-        self.title_mobject = Tex(f"\\textbf{{{title}}}", font_size=36)
-        self.description_mobject = Tex(self.description, font_size=24, tex_environment="markdown", tex_template=MarkdownTexTemplate())
+        self.description = self.description.split("\n")
+        for i in range(1, len(self.description)):
+            self.description[i] = self.description[i].removeprefix(4 * " ")
+        self.description = "\n".join(self.description)
+        self.description.replace("~.", "")
+        self.title = mobject.__class__.__name__ if title is None else title
+        self.title_mobject = Tex(f"\\textbf{{{self.title}}}")
+        self.description_mobject = RstMobject(self.description).scale_to_fit_height(5)
         self.add(self.title_mobject, self.mobject, self.description_mobject)
-        self.arrange(DOWN, buff=0.5)
-        rec_config = rec_config or {
+        buff = 0.5 if buff is None else buff
+        self.arrange(DOWN, buff=buff)
+        rec_config = {
             "stroke_color": WHITE,
             "stroke_width": 2,
             "fill_color": BLACK,
             "fill_opacity": 0.5,
             "buff": 0.2,
             "corner_radius": 0.2
-        }
-        self.add(SurroundingRectangle(self, **rec_config))
-    
-    def set_description(self, description: str):
-        self.description = description
-        self[2].become(Tex(self.description, font_size=24, tex_environment="markdown", tex_template=MarkdownTexTemplate()))
-        return self
-    
-    def set_title(self, title: str):
-        self.title = title
-        self[0].become(Tex(f"\\textbf{{{title}}}", font_size=36))
-        return self
-    
-    def set_mobject(self, mobject: Mobject, description: str | None = None, title: str | None = None):
-        self[1].become(mobject)
-        self.set_description(mobject.__doc__ if description is None else description)
-        self.set_title(mobject.__class__.__name__ or title)
-        return self
+        } if rec_config is None else rec_config
+        self.add_to_back(SurroundingRectangle(self, **rec_config))
+        height = 7 if height is None else height
+        self.scale_to_fit_height(height)
```

### Comparing `manim_course_utils-0.9.0/pyproject.toml` & `manim_course_utils-1.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 [tool.poetry]
 name = "manim-course-utils"
-version = "0.9.0"
+version = "1.0.0"
 description = "Para el curso de ManimCE de MathLike"
 homepage = "https://github.com/MathLike/manim-course-utils"
 repository = "https://github.com/MathLike/manim-course-utils"
 authors = ["MathLike <benjamin.ubilla@uc.cl>"]
 readme = "README.md"
 packages = [{include = "manim_course_utils"}]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.12"
+python = ">=3.8,<3.12"
 manim = "^0.17.3"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `manim_course_utils-0.9.0/PKG-INFO` & `manim_course_utils-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: manim-course-utils
-Version: 0.9.0
+Version: 1.0.0
 Summary: Para el curso de ManimCE de MathLike
 Home-page: https://github.com/MathLike/manim-course-utils
 Author: MathLike
 Author-email: benjamin.ubilla@uc.cl
-Requires-Python: >=3.7,<3.12
+Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: manim (>=0.17.3,<0.18.0)
 Project-URL: Repository, https://github.com/MathLike/manim-course-utils
 Description-Content-Type: text/markdown
```

