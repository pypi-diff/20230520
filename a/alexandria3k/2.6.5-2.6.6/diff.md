# Comparing `tmp/alexandria3k-2.6.5.tar.gz` & `tmp/alexandria3k-2.6.6.tar.gz`

## Comparing `alexandria3k-2.6.5.tar` & `alexandria3k-2.6.6.tar`

### file list

```diff
@@ -1,1153 +1,639 @@
--rw-r--r--   0        0        0    20712 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/.pylintrc
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/Pipfile
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo.sql
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/bin/README.md
--rwxr-xr-x   0        0        0     1071 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/bin/alexandria3k
--rwxr-xr-x   0        0        0      884 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/bin/schema2dot.sed
--rwxr-xr-x   0        0        0      617 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/bin/update-schema
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/.gitignore
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/Makefile
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/api.rst
--rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/cli-eg.rst
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/conf.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/crossref.rst
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/csv_sources.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/debug.rst
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/dev.rst
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/downloading.rst
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/faq.rst
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/index.rst
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/installation.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/make.bat
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/orcid.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/perf.rst
--rw-r--r--   0        0        0     6274 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/python-eg.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/requirements.txt
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/ror.rst
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema.rst
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/use.rst
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/alexandria3k.1
--rw-r--r--   0        0        0    44137 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/.doctrees/environment.pickle
--rw-r--r--   0        0        0    37805 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/.doctrees/index.doctree
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/api.doctree
--rw-r--r--   0        0        0    26359 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/cli-eg.doctree
--rw-r--r--   0        0        0    25477 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/crossref.doctree
--rw-r--r--   0        0        0    24603 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/csv_sources.doctree
--rw-r--r--   0        0        0    19184 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/debug.doctree
--rw-r--r--   0        0        0    12045 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/dev.doctree
--rw-r--r--   0        0        0    13250 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/downloading.doctree
--rw-r--r--   0        0        0   344537 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/faq.doctree
--rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/installation.doctree
--rw-r--r--   0        0        0    14009 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/orcid.doctree
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/perf.doctree
--rw-r--r--   0        0        0    23363 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/python-eg.doctree
--rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/ror.doctree
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/schema.doctree
--rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/use.doctree
--rw-r--r--   0        0        0    71603 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/doctrees/cli/index.doctree
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/.buildinfo
--rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/api.html
--rw-r--r--   0        0        0    34396 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/cli-eg.html
--rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/crossref.html
--rw-r--r--   0        0        0    11708 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/csv_sources.html
--rw-r--r--   0        0        0    10273 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/debug.html
--rw-r--r--   0        0        0    10372 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/dev.html
--rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/downloading.html
--rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/faq.html
--rw-r--r--   0        0        0     8250 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/genindex.html
--rw-r--r--   0        0        0    15686 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/index.html
--rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/installation.html
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/objects.inv
--rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/orcid.html
--rw-r--r--   0        0        0     6243 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/perf.html
--rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/py-modindex.html
--rw-r--r--   0        0        0    22676 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/python-eg.html
--rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/ror.html
--rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/schema.html
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/search.html
--rw-r--r--   0        0        0    21713 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/searchindex.js
--rw-r--r--   0        0        0     5852 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/use.html
--rw-r--r--   0        0        0    86990 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_images/all.svg
--rw-r--r--   0        0        0    17962 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_images/crossref.svg
--rw-r--r--   0        0        0    29731 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_images/orcid.svg
--rw-r--r--   0        0        0    24792 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_images/other.svg
--rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_images/ror.svg
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/api.rst.txt
--rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/cli-eg.rst.txt
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/crossref.rst.txt
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/csv_sources.rst.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/debug.rst.txt
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/dev.rst.txt
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/downloading.rst.txt
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/faq.rst.txt
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/installation.rst.txt
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/orcid.rst.txt
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/perf.rst.txt
--rw-r--r--   0        0        0     6505 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/python-eg.rst.txt
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/ror.rst.txt
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/schema.rst.txt
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/use.rst.txt
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_sources/cli/index.rst.txt
--rw-r--r--   0        0        0    11230 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_static/alabaster.css
--rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0    11577 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/_build/html/cli/index.html
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/cli/index.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/.gitignore
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/README.md
--rw-r--r--   0        0        0    49937 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/all.pdf
--rw-r--r--   0        0        0    86990 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/all.svg
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/crossref.dot
--rw-r--r--   0        0        0    33919 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/crossref.pdf
--rw-r--r--   0        0        0    17962 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/crossref.svg
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/orcid.dot
--rw-r--r--   0        0        0    34882 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/orcid.pdf
--rw-r--r--   0        0        0    29731 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/orcid.svg
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/other.dot
--rw-r--r--   0        0        0    40679 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/other.pdf
--rw-r--r--   0        0        0    24792 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/other.svg
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/ror.dot
--rw-r--r--   0        0        0    32800 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/ror.pdf
--rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/ror.svg
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/docs/schema/schema-head.dot
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/README.md
--rwxr-xr-x   0        0        0      215 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/test-all.sh
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/author-productivity/.gitignore
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/author-productivity/Makefile
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/author-productivity/README.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/author-productivity/author-productivity.sql
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/author-productivity/frequent-names.sql
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/author-productivity/yearly_authors.rdbu
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/author-productivity/yearly_authors.sql
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/author-productivity/yearly_works.sql
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/authors-by-decade/.gitignore
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/authors-by-decade/Makefile
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/authors-by-decade/README.md
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/authors-by-decade/authors-by-decade.sql
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/authors-by-decade/num_work_authors.sql
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cdindex/.gitignore
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cdindex/Makefile
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cdindex/README.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cdindex/cd5index-all.sql
--rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cdindex/cdindex-db.cpp
--rwxr-xr-x   0        0        0     4428 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cdindex/cdindex-db.py
--rwxr-xr-x   0        0        0     2028 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cdindex/cdindex-otf.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cdindex/nature-example.sql
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cdindex/yearly-cdindex.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/common/.gitignore
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/common/Makefile
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/common/unit-test/README.md
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/common/unit-test/works-subjects.rdbu
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/.depend
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/.depend.all
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/.gitignore
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/Makefile
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/README.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/author-number-quartiles.sql
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/funders.sql
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/inner-citations.sql
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/number-of-authors.sql
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/number-of-works.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/rolap
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/subjects.sql
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/work-affiliations.rdbu
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/work-affiliations.sql
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/LICENSE
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/Makefile
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/README.md
--rwxr-xr-x   0        0        0     1899 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/create_db.sh
--rwxr-xr-x   0        0        0     1076 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/dep2dot.sed
--rwxr-xr-x   0        0        0      759 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/dep2tsort.sed
--rwxr-xr-x   0        0        0     1426 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/drop_db.sh
--rwxr-xr-x   0        0        0     3114 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/mkdep.sh
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/mktags.sh
--rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/need_var.sh
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/psql-ctime.sql
--rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/run_sql.sh
--rwxr-xr-x   0        0        0     2363 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/run_test.sh
--rwxr-xr-x   0        0        0      963 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/sync_timestamps.sh
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/.gitignore
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/Makefile
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/forked_projects.sql
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/popular_projects.sql
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/pr_projects.sql
--rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sh
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sql
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_stars.sql
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_urls.sql
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_commit_projects.sql
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_issue_projects.sql
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/.gitignore
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/Makefile
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.rdbu
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.sql
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.rdbu
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.sql
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.rdbu
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.sql
--rwxr-xr-x   0        0        0      457 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sh
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sql
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.rdbu
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.sql
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.rdbu
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.sql
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.rdbu
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.sql
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.rdbu
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.sql
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/crossref-standalone/.gitignore
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/crossref-standalone/Makefile
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/crossref-standalone/README.md
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/crossref-standalone/work-metrics.sql
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/crossref-standalone/yearly-abstracts.rdbu
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/crossref-standalone/yearly-abstracts.sql
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/crossref-standalone/yearly-journals.rdbu
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/crossref-standalone/yearly-journals.sql
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cs_cdindex/.gitignore
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cs_cdindex/Makefile
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cs_cdindex/cdindex-by-type.sql
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cs_cdindex/cdindex.sql
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cs_cdindex/citations_number.sql
--rwxr-xr-x   0        0        0      551 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cs_cdindex/cs_works.sed
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cs_cdindex/references_number.sql
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cs_cdindex/top-consolidating.sql
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/cs_cdindex/top-disruptive.sql
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/.depend
--rw-r--r--   0        0        0     6143 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/.depend.all
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/.gitignore
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/Makefile
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/asjcs
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/author-number-quartiles-2020.sql
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/author-number-quartiles-medicine-2020.sql
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/author-number-quartiles-medicine.sql
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/author-number-quartiles.sql
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/author_year_works.rdbu
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/author_year_works.sql
--rw-r--r--   0        0        0   105893 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/fields_by_year.svg
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/general-field-publications-list.sql
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/general_field_publications.sql
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/graph.dot
--rw-r--r--   0        0        0   133883 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/graph.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/link-works-asjcs
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/metrics.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/populate
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/prolific-authors.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/rolap
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/subject-hierarchy-list.sql
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/subject_hierarchy.sql
--rw-r--r--   0        0        0   292745 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/subject_hierarchy.svg
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/subject_pair_fundamentalness_percentile.sql
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/subject_pair_strength_percentile.sql
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/sustainable-authors.rdbu
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/sustainable-authors.sql
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/twenty_year_citations.sql
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/twenty_year_publications.rdbu
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/twenty_year_publications.sql
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/two_year_citations.rdbu
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/two_year_citations.sql
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/work_subject_citations.rdbu
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/work_subject_citations.sql
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/work_subject_numbers.sql
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-20y-impact-factor.sql
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-2y-impact-factor.sql
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-author-affiliations.sql
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-authors-orcid.sql
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-authors-per-work.sql
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-citations-per-paper.rdbu
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-citations-per-paper.sql
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-funder-awards.sql
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-funders-doi.sql
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-proportion-of-cited-papers.rdbu
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-proportion-of-cited-papers.sql
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-references-doi.sql
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-references-per-paper.rdbu
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-references-per-paper.sql
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-work-authors.sql
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-work-funders.sql
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-work-links.rdbu
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-work-links.sql
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-work-references.sql
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-work-subjects.sql
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly-works.sql
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/yearly_works_all.sql
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/reports/metrics.txt
--rw-r--r--   0        0        0    19721 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/reports/subject_hierarchy.svg
--rw-r--r--   0        0        0   400154 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/reports/subject_hierarchy.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/LICENSE
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/Makefile
--rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/README.md
--rwxr-xr-x   0        0        0     1899 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/create_db.sh
--rwxr-xr-x   0        0        0     1076 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/dep2dot.sed
--rwxr-xr-x   0        0        0      759 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/dep2tsort.sed
--rwxr-xr-x   0        0        0     1426 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/drop_db.sh
--rwxr-xr-x   0        0        0     3114 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/mkdep.sh
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/mktags.sh
--rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/need_var.sh
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/psql-ctime.sql
--rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/run_sql.sh
--rwxr-xr-x   0        0        0     2049 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/run_test.sh
--rwxr-xr-x   0        0        0      963 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/sync_timestamps.sh
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/.gitignore
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/Makefile
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/forked_projects.sql
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/popular_projects.sql
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/pr_projects.sql
--rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sh
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sql
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_stars.sql
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_urls.sql
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_commit_projects.sql
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_issue_projects.sql
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/.gitignore
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/Makefile
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.rdbu
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.sql
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.rdbu
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.sql
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.rdbu
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.sql
--rwxr-xr-x   0        0        0      457 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sh
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sql
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.rdbu
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.sql
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.rdbu
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.sql
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.rdbu
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.sql
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.rdbu
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/tables/general_field_publications
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/tables/subject_pair_fundamentalness_percentile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/tables/subject_pair_strength_percentile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/tables/work_subject_citations
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/tables/work_subject_numbers
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/unit-test/README.md
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/unit-test/subject-pair-strength-percentile.rdbu
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/graph/unit-test/work_subject_citations.svg
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/.depend
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/.depend.all
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/.gitignore
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/Makefile
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/README.md
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/citable_works.rdbu
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/citable_works.sql
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/citations.rdbu
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/citations.sql
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/impact-factor-all.rdbu
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/impact-factor-all.sql
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/impact-factor-non-review.sql
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/impact-factor-top.sql
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/impact_factor.rdbu
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/impact_factor.sql
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/impact_factor_titles.sql
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/most-cited-3y.sql
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/most-cited-in-3y.sql
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/publications.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/rolap
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/works_issn.rdbu
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/works_issn.sql
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/LICENSE
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/Makefile
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/README.md
--rwxr-xr-x   0        0        0     1899 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/create_db.sh
--rwxr-xr-x   0        0        0     1076 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/dep2dot.sed
--rwxr-xr-x   0        0        0      759 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/dep2tsort.sed
--rwxr-xr-x   0        0        0     1426 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/drop_db.sh
--rwxr-xr-x   0        0        0     3114 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/mkdep.sh
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/mktags.sh
--rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/need_var.sh
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/psql-ctime.sql
--rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/run_sql.sh
--rwxr-xr-x   0        0        0     2363 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/run_test.sh
--rwxr-xr-x   0        0        0      963 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/sync_timestamps.sh
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/.gitignore
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/Makefile
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/forked_projects.sql
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/popular_projects.sql
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/pr_projects.sql
--rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sh
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sql
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_stars.sql
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_urls.sql
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_commit_projects.sql
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_issue_projects.sql
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/.gitignore
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/Makefile
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.rdbu
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.sql
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.rdbu
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.sql
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.rdbu
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.sql
--rwxr-xr-x   0        0        0      457 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sh
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sql
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.rdbu
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.sql
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.rdbu
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.sql
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.rdbu
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.sql
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.rdbu
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.sql
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/.depend
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/.depend.all
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/.gitignore
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/Makefile
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/README.md
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/issn_h5.rdbu
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/issn_h5.sql
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/journal-h5-all.sql
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/journal-h5.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/rolap
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/work_citations.rdbu
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/work_citations.sql
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/works_issn.rdbu
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/works_issn.sql
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/LICENSE
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/Makefile
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/README.md
--rwxr-xr-x   0        0        0     1899 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/create_db.sh
--rwxr-xr-x   0        0        0     1076 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/dep2dot.sed
--rwxr-xr-x   0        0        0      759 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/dep2tsort.sed
--rwxr-xr-x   0        0        0     1426 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/drop_db.sh
--rwxr-xr-x   0        0        0     3114 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/mkdep.sh
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/mktags.sh
--rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/need_var.sh
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/psql-ctime.sql
--rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/run_sql.sh
--rwxr-xr-x   0        0        0     2363 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/run_test.sh
--rwxr-xr-x   0        0        0      963 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/sync_timestamps.sh
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/.gitignore
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/Makefile
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/forked_projects.sql
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/popular_projects.sql
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/pr_projects.sql
--rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sh
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sql
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_stars.sql
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_urls.sql
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_commit_projects.sql
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_issue_projects.sql
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/.gitignore
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/Makefile
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.rdbu
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.sql
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.rdbu
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.sql
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.rdbu
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.sql
--rwxr-xr-x   0        0        0      457 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sh
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sql
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.rdbu
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.sql
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.rdbu
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.sql
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.rdbu
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.sql
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.rdbu
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.sql
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/orcid/.gitignore
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/orcid/Makefile
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/orcid/README.md
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/orcid/metrics.sql
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/.depend
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/.depend.all
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/.gitignore
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/Makefile
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/README.md
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/citation-graph-indexes.sql
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/citation-graph.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/orcid-h5.sql
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/orcid_h5.rdbu
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/orcid_h5.sql
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/random_other_works.sql
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/random_top_works.rdbu
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/random_top_works.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/rolap
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/work_citations.rdbu
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/work_citations.sql
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/works_orcid.rdbu
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/works_orcid.sql
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/LICENSE
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/Makefile
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/README.md
--rwxr-xr-x   0        0        0     1899 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/create_db.sh
--rwxr-xr-x   0        0        0     1076 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/dep2dot.sed
--rwxr-xr-x   0        0        0      759 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/dep2tsort.sed
--rwxr-xr-x   0        0        0     1426 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/drop_db.sh
--rwxr-xr-x   0        0        0     3114 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/mkdep.sh
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/mktags.sh
--rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/need_var.sh
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/psql-ctime.sql
--rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/run_sql.sh
--rwxr-xr-x   0        0        0     2363 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/run_test.sh
--rwxr-xr-x   0        0        0      963 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/sync_timestamps.sh
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/.gitignore
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/Makefile
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/forked_projects.sql
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/popular_projects.sql
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/pr_projects.sql
--rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sh
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sql
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_stars.sql
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_urls.sql
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_commit_projects.sql
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_issue_projects.sql
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/.gitignore
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/Makefile
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.rdbu
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.sql
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.rdbu
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.sql
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.rdbu
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.sql
--rwxr-xr-x   0        0        0      457 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sh
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sql
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.rdbu
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.sql
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.rdbu
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.sql
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.rdbu
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.sql
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.rdbu
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.sql
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/research-synthesis/.gitignore
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/research-synthesis/Makefile
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/research-synthesis/README.md
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/research-synthesis/early-studies.sql
--rw-r--r--   0        0        0    21448 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/research-synthesis/research-synthesis.png
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/research-synthesis/research-synthesis.sql
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/sample/.gitignore
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/sample/Makefile
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/sample/README.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/sample/indexes.sql
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/soft-eng-h5/.gitignore
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/soft-eng-h5/Makefile
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/soft-eng-h5/README.md
--rw-r--r--   0        0        0     5915 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/soft-eng-h5/se-5y.sql
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/soft-eng-h5/venue-h5-report.sql
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/soft-eng-h5/venue_h5.sql
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/soft-eng-h5/work_citations.sql
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/soft-eng-h5/works_venue.sql
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/tawfik/.gitignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/tawfik/Makefile
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/tawfik/README.md
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/tawfik/baseline_cdindex.sql
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/tawfik/comparison-report.sql
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/tawfik/comparison.sql
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/tawfik/tawfik-works.sql
--rw-r--r--   0        0        0    16765 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/tawfik/tawfik-works.txt
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/tawfik/tawfik_cdindex.sql
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/tawfik/tawfik_works.sql
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/yearly-numpages/.gitignore
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/yearly-numpages/Makefile
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/yearly-numpages/README.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/yearly-numpages/works_pages.rdbu
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/yearly-numpages/works_pages.sql
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/examples/yearly-numpages/yearly-numpages.sql
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/pyvenv.cfg
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/bin/Activate.ps1
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/bin/activate
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/bin/activate.csh
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/bin/activate.fish
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/bin/alexandria3k
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/bin/easy_install
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/bin/easy_install-3.9
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/bin/pip
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/bin/pip3
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/bin/pip3.9
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/bin/python -> /cygdrive/c/dds/home/.local/share/virtualenvs/src-caGTairT/bin/python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/bin/python3.9 -> python
--rwxr-xr-x   0        0        0   293764 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/ahocorasick.cpython-39-x86_64-cygwin.dll
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/easy_install.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/__init__.py
--rwxr-xr-x   0        0        0    17547 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/__main__.py
--rwxr-xr-x   0        0        0     5399 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/common.py
--rw-r--r--   0        0        0    48543 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/crossref.py
--rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/csv_sources.py
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/debug.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/file_cache.py
--rw-r--r--   0        0        0    23397 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/orcid.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/perf.py
--rw-r--r--   0        0        0    11882 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/ror.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/tsort.py
--rw-r--r--   0        0        0    14968 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/virtual_db.py
--rw-r--r--   0        0        0    16464 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/data/asjc.csv
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/sql/link-works-asjcs.sql
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/sql/normalize-asjc.sql
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/sql/normalize-doaj.sql
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/sql/normalize-journal-names-issns.sql
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/sql/work-authors-top-rors.sql
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k-2.6.4.dist-info/INSTALLER
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k-2.6.4.dist-info/METADATA
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k-2.6.4.dist-info/RECORD
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k-2.6.4.dist-info/WHEEL
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k-2.6.4.dist-info/entry_points.txt
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k-2.6.4.dist-info/licenses/LICENSE
--rwxr-xr-x   0        0        0 10215168 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/apsw/__init__.cpython-39-x86_64-cygwin.dll
--rw-r--r--   0        0        0   197070 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/apsw/__init__.pyi
--rwxr-xr-x   0        0        0       60 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/apsw/__main__.py
--rw-r--r--   0        0        0    55327 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/apsw/ext.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/apsw/py.typed
--rwxr-xr-x   0        0        0   121056 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/apsw/shell.py
--rwxr-xr-x   0        0        0    19327 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/apsw/speedtest.py
--rwxr-xr-x   0        0        0   387461 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/apsw/tests.py
--rwxr-xr-x   0        0        0    12493 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/apsw/trace.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/apsw-3.41.2.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/apsw-3.41.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/apsw-3.41.2.0.dist-info/METADATA
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/apsw-3.41.2.0.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/apsw-3.41.2.0.dist-info/WHEEL
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/apsw-3.41.2.0.dist-info/top_level.txt
--rw-r--r--   0        0        0    26518 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata/__init__.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata/_adapters.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata/_collections.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata/_compat.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata/_functools.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata/_itertools.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata/_meta.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata/_py39compat.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata/_text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata/py.typed
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata-6.1.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata-6.1.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata-6.1.0.dist-info/METADATA
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata-6.1.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata-6.1.0.dist-info/WHEEL
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/importlib_metadata-6.1.0.dist-info/top_level.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/__init__.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/__main__.py
--rwxr-xr-x   0        0        0     2797 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    14076 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    43323 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/download.py
--rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0    56017 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/index.py
--rw-r--r--   0        0        0    17303 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/legacy_resolve.py
--rw-r--r--   0        0        0     5045 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/locations.py
--rw-r--r--   0        0        0    13220 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/pep425tags.py
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0    42309 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/wheel.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0    13029 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    27543 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     8156 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0    22646 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    10497 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     6977 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/distributions/source.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     6553 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     5224 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9680 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    11728 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    11858 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    14180 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    40296 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/req/req_tracker.py
--rw-r--r--   0        0        0    23105 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     9398 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0    12883 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/marker_files.py
--rw-r--r--   0        0        0    38796 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     6292 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/outdated.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/typing.py
--rw-r--r--   0        0        0    13768 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/ui.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11697 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    19010 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/__init__.py
--rwxr-xr-x   0        0        0    24547 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/appdirs.py
--rw-r--r--   0        0        0    43251 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distro.py
--rw-r--r--   0        0        0    79852 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/ipaddress.py
--rw-r--r--   0        0        0   245385 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pyparsing.py
--rw-r--r--   0        0        0     9972 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/retrying.py
--rw-r--r--   0        0        0    32452 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0        0        0    13698 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31254 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0     9411 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/compat.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    31621 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20715 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    13838 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25777 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    19643 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0    12839 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    17948 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/langcyrillicmodel.py
--rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0    12592 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    25481 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    12485 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/cli/__init__.py
--rwxr-xr-x   0        0        0     2774 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    10462 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41404 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51029 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    21066 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51807 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    40234 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10766 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/scripts.py
--rwxr-xr-x   0        0        0    92672 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/t32.exe
--rwxr-xr-x   0        0        0   102912 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    59790 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23391 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/version.py
--rwxr-xr-x   0        0        0    89088 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/w32.exe
--rwxr-xr-x   0        0        0    99840 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    40437 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/_backport/__init__.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/_backport/misc.py
--rw-r--r--   0        0        0    25647 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/_backport/shutil.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/_backport/sysconfig.cfg
--rw-r--r--   0        0        0    26964 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/_backport/sysconfig.py
--rw-r--r--   0        0        0    92628 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/distlib/_backport/tarfile.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/__init__.py
--rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/_ihatexml.py
--rw-r--r--   0        0        0    32552 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/_inputstream.py
--rw-r--r--   0        0        0    76580 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/_tokenizer.py
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/_utils.py
--rw-r--r--   0        0        0    83518 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/constants.py
--rw-r--r--   0        0        0   118963 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/html5parser.py
--rw-r--r--   0        0        0    15758 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/serializer.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/_trie/__init__.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/_trie/_base.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/_trie/datrie.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/_trie/py.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/__init__.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/base.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/lint.py
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/optionaltags.py
--rw-r--r--   0        0        0    26248 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/sanitizer.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/filters/whitespace.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/treeadapters/sax.py
--rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
--rw-r--r--   0        0        0    14579 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/treebuilders/base.py
--rw-r--r--   0        0        0     8925 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/treebuilders/dom.py
--rw-r--r--   0        0        0    12764 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/treebuilders/etree.py
--rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
--rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py
--rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/treewalkers/base.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/treewalkers/dom.py
--rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/treewalkers/etree.py
--rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    11733 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    40899 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0   198292 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/lockfile/__init__.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/lockfile/linklockfile.py
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/lockfile/mkdirlockfile.py
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/lockfile/pidlockfile.py
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/lockfile/sqlitelockfile.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/lockfile/symlinklockfile.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/msgpack/_version.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0    37491 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/packaging/_compat.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8234 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    27778 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pep517/__init__.py
--rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pep517/_in_process.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pep517/build.py
--rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pep517/check.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pep517/colorlog.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pep517/compat.py
--rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pep517/envbuild.py
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pep517/wrappers.py
--rw-r--r--   0        0        0   107910 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pkg_resources/py31compat.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/progress/__init__.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/progress/bar.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/progress/counter.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/progress/spinner.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pytoml/__init__.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pytoml/core.py
--rw-r--r--   0        0        0    10326 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pytoml/parser.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pytoml/test.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pytoml/utils.py
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/pytoml/writer.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    21548 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10206 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/auth.py
--rwxr-xr-x   0        0        0      465 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18430 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    34275 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    29332 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    30049 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10746 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0    15001 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    35307 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    17050 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    27171 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    16468 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    32826 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17576 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    30098 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/rfc3986/__init__.py
--rw-r--r--   0        0        0    13214 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/rfc3986/_mixin.py
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/rfc3986/abnf_regexp.py
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/rfc3986/api.py
--rw-r--r--   0        0        0     9577 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/rfc3986/builder.py
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/rfc3986/compat.py
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/rfc3986/exceptions.py
--rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/rfc3986/iri.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/rfc3986/misc.py
--rw-r--r--   0        0        0     5259 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/rfc3986/normalizers.py
--rw-r--r--   0        0        0    14654 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/rfc3986/parseresult.py
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/rfc3986/uri.py
--rw-r--r--   0        0        0    13854 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/rfc3986/validators.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
--rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    15150 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    13798 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip-19.2.3.dist-info/INSTALLER
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip-19.2.3.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip-19.2.3.dist-info/METADATA
--rw-r--r--   0        0        0    51599 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip-19.2.3.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip-19.2.3.dist-info/WHEEL
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip-19.2.3.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip-19.2.3.dist-info/top_level.txt
--rw-r--r--   0        0        0   108309 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/__init__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/py31compat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/_vendor/__init__.py
--rwxr-xr-x   0        0        0    24701 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/_vendor/appdirs.py
--rw-r--r--   0        0        0   232055 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/_vendor/pyparsing.py
--rw-r--r--   0        0        0    30098 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/_vendor/six.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/_compat.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    28025 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pyahocorasick-2.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pyahocorasick-2.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0    13634 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pyahocorasick-2.0.0.dist-info/METADATA
--rw-r--r--   0        0        0    12136 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pyahocorasick-2.0.0.dist-info/README.rst
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pyahocorasick-2.0.0.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pyahocorasick-2.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pyahocorasick-2.0.0.dist-info/top_level.txt
--rw-r--r--   0        0        0     7283 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/_deprecation_warning.py
--rw-r--r--   0        0        0     6592 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/archive_util.py
--rw-r--r--   0        0        0     9597 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/build_meta.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/cli-32.exe
--rwxr-xr-x   0        0        0    74752 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/cli-64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/cli.exe
--rw-r--r--   0        0        0    20425 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/config.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/dep_util.py
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/depends.py
--rw-r--r--   0        0        0    50248 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/dist.py
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/extension.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/glibc.py
--rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/glob.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/gui-32.exe
--rwxr-xr-x   0        0        0    75264 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/gui-64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/gui.exe
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/launch.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/lib2to3_ex.py
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/monkey.py
--rw-r--r--   0        0        0    40838 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/msvc.py
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/namespaces.py
--rw-r--r--   0        0        0    40587 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/package_index.py
--rw-r--r--   0        0        0    10861 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/pep425tags.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/py27compat.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/py31compat.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/py33compat.py
--rw-r--r--   0        0        0    14276 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/sandbox.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/script.tmpl
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/site-patch.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/ssl_support.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/version.py
--rw-r--r--   0        0        0     8094 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/wheel.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/windows_support.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0        0        0   232055 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/_vendor/pyparsing.py
--rw-r--r--   0        0        0    30098 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/_vendor/six.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/_vendor/packaging/_compat.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    28025 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/__init__.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/alias.py
--rw-r--r--   0        0        0    18167 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/bdist_wininst.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0        0        0    13019 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/build_py.py
--rw-r--r--   0        0        0     8184 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/develop.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/dist_info.py
--rwxr-xr-x   0        0        0    87273 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0        0        0    25570 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/install.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/register.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/rotate.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/sdist.py
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/setopt.py
--rw-r--r--   0        0        0     9285 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/test.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/upload.py
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools-41.2.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools-41.2.0.dist-info/LICENSE
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools-41.2.0.dist-info/METADATA
--rw-r--r--   0        0        0    13853 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools-41.2.0.dist-info/RECORD
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools-41.2.0.dist-info/WHEEL
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools-41.2.0.dist-info/dependency_links.txt
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools-41.2.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools-41.2.0.dist-info/top_level.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/setuptools-41.2.0.dist-info/zip-safe
--rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/zipp/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/zipp/py310compat.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/zipp-3.15.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/zipp-3.15.0.dist-info/LICENSE
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/zipp-3.15.0.dist-info/METADATA
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/zipp-3.15.0.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/zipp-3.15.0.dist-info/WHEEL
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/foo/lib/python3.9/site-packages/zipp-3.15.0.dist-info/top_level.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/.gitignore
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/Pipfile
--rw-r--r--   0        0        0    46118 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/Pipfile.lock
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/__init__.py
--rwxr-xr-x   0        0        0    17839 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/__main__.py
--rwxr-xr-x   0        0        0     5399 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/common.py
--rw-r--r--   0        0        0    48543 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/crossref.py
--rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/csv_sources.py
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/debug.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/file_cache.py
--rw-r--r--   0        0        0    23397 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/orcid.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/perf.py
--rw-r--r--   0        0        0    11882 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/ror.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/tsort.py
--rw-r--r--   0        0        0    14968 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/virtual_db.py
--rw-r--r--   0        0        0    16464 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/data/asjc.csv
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/sql/link-works-asjcs.sql
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/sql/normalize-asjc.sql
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/sql/normalize-doaj.sql
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/sql/normalize-journal-names-issns.sql
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/src/alexandria3k/sql/work-authors-top-rors.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/__init__.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/link-works-asjcs.rdbu
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/normalize-asjc-general-fields.rdbu
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/normalize-asjc-subject-areas.rdbu
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/normalize-asjc.rdbu
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/regression.sh
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/test_common.py
--rw-r--r--   0        0        0    19056 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/test_crossref.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/test_csv_sources.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/test_debug.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/test_dir.py
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/test_journal_names.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/test_main.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/test_orcid.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/test_perf.py
--rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/test_ror.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/test_tsort.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/test_virtual_db.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/work-authors-top-rors.rdbu
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/chat/chat.rdbu
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/chat/fixed.rdbu
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/chat/foo.sql
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/chat/sqlite3
--rw-r--r--   0        0        0   115459 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/data/ORCID_2022_10_summaries.tar.gz
--rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/data/ror.zip
--rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/data/titleFile.csv
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/data/sample/1item.json.gz
--rw-r--r--   0        0        0     8634 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/data/sample/2item-references.json.gz
--rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/data/sample/3items.json.gz
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/data/sample/affiliations.json.gz
--rw-r--r--   0        0        0    10950 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/data/sample/funded.json.gz
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/data/sample/orcid-work.json.gz
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/data/sample/same-author.json.gz
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/data/sample/updated.json.gz
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/tests/tmp/README.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/LICENSE
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/README.md
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/pyproject.toml
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 alexandria3k-2.6.5/PKG-INFO
+-rw-r--r--   0        0        0    20712 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/.pylintrc
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/bin/README.md
+-rwxr-xr-x   0        0        0     1071 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/bin/alexandria3k
+-rwxr-xr-x   0        0        0      884 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/bin/schema2dot.sed
+-rwxr-xr-x   0        0        0      617 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/bin/update-schema
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/.gitignore
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/Makefile
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/api.rst
+-rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/cli-eg.rst
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/conf.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/crossref.rst
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/csv_sources.rst
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/debug.rst
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/dev.rst
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/downloading.rst
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/faq.rst
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/index.rst
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/installation.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/make.bat
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/orcid.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/perf.rst
+-rw-r--r--   0        0        0     6274 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/python-eg.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/requirements.txt
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/ror.rst
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema.rst
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/use.rst
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/alexandria3k.1
+-rw-r--r--   0        0        0    44137 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/.doctrees/environment.pickle
+-rw-r--r--   0        0        0    37805 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/.doctrees/index.doctree
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/api.doctree
+-rw-r--r--   0        0        0    26359 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/cli-eg.doctree
+-rw-r--r--   0        0        0    25477 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/crossref.doctree
+-rw-r--r--   0        0        0    24603 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/csv_sources.doctree
+-rw-r--r--   0        0        0    19184 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/debug.doctree
+-rw-r--r--   0        0        0    12045 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/dev.doctree
+-rw-r--r--   0        0        0    13250 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/downloading.doctree
+-rw-r--r--   0        0        0   344537 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/faq.doctree
+-rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/installation.doctree
+-rw-r--r--   0        0        0    14009 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/orcid.doctree
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/perf.doctree
+-rw-r--r--   0        0        0    23363 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/python-eg.doctree
+-rw-r--r--   0        0        0    12914 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/ror.doctree
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/schema.doctree
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/use.doctree
+-rw-r--r--   0        0        0    71603 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/doctrees/cli/index.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/.buildinfo
+-rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/api.html
+-rw-r--r--   0        0        0    34396 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/cli-eg.html
+-rw-r--r--   0        0        0    11284 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/crossref.html
+-rw-r--r--   0        0        0    11708 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/csv_sources.html
+-rw-r--r--   0        0        0    10273 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/debug.html
+-rw-r--r--   0        0        0    10372 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/dev.html
+-rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/downloading.html
+-rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/faq.html
+-rw-r--r--   0        0        0     8250 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/genindex.html
+-rw-r--r--   0        0        0    15686 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/index.html
+-rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/installation.html
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/objects.inv
+-rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/orcid.html
+-rw-r--r--   0        0        0     6243 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/perf.html
+-rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/py-modindex.html
+-rw-r--r--   0        0        0    22676 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/python-eg.html
+-rw-r--r--   0        0        0     7965 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/ror.html
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/schema.html
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/search.html
+-rw-r--r--   0        0        0    21713 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/searchindex.js
+-rw-r--r--   0        0        0     5852 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/use.html
+-rw-r--r--   0        0        0    86990 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_images/all.svg
+-rw-r--r--   0        0        0    17962 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_images/crossref.svg
+-rw-r--r--   0        0        0    29731 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_images/orcid.svg
+-rw-r--r--   0        0        0    24792 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_images/other.svg
+-rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_images/ror.svg
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/api.rst.txt
+-rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/cli-eg.rst.txt
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/crossref.rst.txt
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/csv_sources.rst.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/debug.rst.txt
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/dev.rst.txt
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/downloading.rst.txt
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/faq.rst.txt
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/installation.rst.txt
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/orcid.rst.txt
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/perf.rst.txt
+-rw-r--r--   0        0        0     6505 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/python-eg.rst.txt
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/ror.rst.txt
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/schema.rst.txt
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/use.rst.txt
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_sources/cli/index.rst.txt
+-rw-r--r--   0        0        0    11230 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_static/doctools.js
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_static/plus.png
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0    11577 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/_build/html/cli/index.html
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/cli/index.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/.gitignore
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/README.md
+-rw-r--r--   0        0        0    49937 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/all.pdf
+-rw-r--r--   0        0        0    86990 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/all.svg
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/crossref.dot
+-rw-r--r--   0        0        0    33919 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/crossref.pdf
+-rw-r--r--   0        0        0    17962 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/crossref.svg
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/orcid.dot
+-rw-r--r--   0        0        0    34882 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/orcid.pdf
+-rw-r--r--   0        0        0    29731 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/orcid.svg
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/other.dot
+-rw-r--r--   0        0        0    40679 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/other.pdf
+-rw-r--r--   0        0        0    24792 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/other.svg
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/ror.dot
+-rw-r--r--   0        0        0    32800 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/ror.pdf
+-rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/ror.svg
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/docs/schema/schema-head.dot
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/README.md
+-rwxr-xr-x   0        0        0      215 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/test-all.sh
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/author-productivity/.gitignore
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/author-productivity/Makefile
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/author-productivity/README.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/author-productivity/author-productivity.sql
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/author-productivity/frequent-names.sql
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/author-productivity/yearly_authors.rdbu
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/author-productivity/yearly_authors.sql
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/author-productivity/yearly_works.sql
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/authors-by-decade/.gitignore
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/authors-by-decade/Makefile
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/authors-by-decade/README.md
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/authors-by-decade/authors-by-decade.sql
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/authors-by-decade/num_work_authors.sql
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cdindex/.gitignore
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cdindex/Makefile
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cdindex/README.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cdindex/cd5index-all.sql
+-rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cdindex/cdindex-db.cpp
+-rwxr-xr-x   0        0        0     4428 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cdindex/cdindex-db.py
+-rwxr-xr-x   0        0        0     2028 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cdindex/cdindex-otf.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cdindex/nature-example.sql
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cdindex/yearly-cdindex.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/common/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/common/Makefile
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/common/unit-test/README.md
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/common/unit-test/works-subjects.rdbu
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/.depend
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/.depend.all
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/.gitignore
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/Makefile
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/README.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/author-number-quartiles.sql
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/funders.sql
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/inner-citations.sql
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/number-of-authors.sql
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/number-of-works.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/rolap
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/subjects.sql
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/work-affiliations.rdbu
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/work-affiliations.sql
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/LICENSE
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/Makefile
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/README.md
+-rwxr-xr-x   0        0        0     1899 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/create_db.sh
+-rwxr-xr-x   0        0        0     1076 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/dep2dot.sed
+-rwxr-xr-x   0        0        0      759 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/dep2tsort.sed
+-rwxr-xr-x   0        0        0     1426 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/drop_db.sh
+-rwxr-xr-x   0        0        0     3114 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/mkdep.sh
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/mktags.sh
+-rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/need_var.sh
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/psql-ctime.sql
+-rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/run_sql.sh
+-rwxr-xr-x   0        0        0     2363 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/run_test.sh
+-rwxr-xr-x   0        0        0      963 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/sync_timestamps.sh
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/.gitignore
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/Makefile
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/forked_projects.sql
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/popular_projects.sql
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/pr_projects.sql
+-rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sh
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sql
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_stars.sql
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_urls.sql
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_commit_projects.sql
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_issue_projects.sql
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/.gitignore
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/Makefile
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.rdbu
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.sql
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.rdbu
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.sql
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.rdbu
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.sql
+-rwxr-xr-x   0        0        0      457 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sh
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sql
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.rdbu
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.sql
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.rdbu
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.sql
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.rdbu
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.sql
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.rdbu
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/covid/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.sql
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/crossref-standalone/.gitignore
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/crossref-standalone/Makefile
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/crossref-standalone/README.md
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/crossref-standalone/work-metrics.sql
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/crossref-standalone/yearly-abstracts.rdbu
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/crossref-standalone/yearly-abstracts.sql
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/crossref-standalone/yearly-journals.rdbu
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/crossref-standalone/yearly-journals.sql
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cs_cdindex/.gitignore
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cs_cdindex/Makefile
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cs_cdindex/cdindex-by-type.sql
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cs_cdindex/cdindex.sql
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cs_cdindex/citations_number.sql
+-rwxr-xr-x   0        0        0      551 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cs_cdindex/cs_works.sed
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cs_cdindex/references_number.sql
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cs_cdindex/top-consolidating.sql
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/cs_cdindex/top-disruptive.sql
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/.depend
+-rw-r--r--   0        0        0     6143 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/.depend.all
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/.gitignore
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/Makefile
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/asjcs
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/author-number-quartiles-2020.sql
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/author-number-quartiles-medicine-2020.sql
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/author-number-quartiles-medicine.sql
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/author-number-quartiles.sql
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/author_year_works.rdbu
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/author_year_works.sql
+-rw-r--r--   0        0        0   105893 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/fields_by_year.svg
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/general-field-publications-list.sql
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/general_field_publications.sql
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/graph.dot
+-rw-r--r--   0        0        0   133883 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/graph.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/link-works-asjcs
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/metrics.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/populate
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/prolific-authors.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/rolap
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/subject-hierarchy-list.sql
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/subject_hierarchy.sql
+-rw-r--r--   0        0        0   292745 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/subject_hierarchy.svg
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/subject_pair_fundamentalness_percentile.sql
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/subject_pair_strength_percentile.sql
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/sustainable-authors.rdbu
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/sustainable-authors.sql
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/twenty_year_citations.sql
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/twenty_year_publications.rdbu
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/twenty_year_publications.sql
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/two_year_citations.rdbu
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/two_year_citations.sql
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/work_subject_citations.rdbu
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/work_subject_citations.sql
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/work_subject_numbers.sql
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-20y-impact-factor.sql
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-2y-impact-factor.sql
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-author-affiliations.sql
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-authors-orcid.sql
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-authors-per-work.sql
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-citations-per-paper.rdbu
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-citations-per-paper.sql
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-funder-awards.sql
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-funders-doi.sql
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-proportion-of-cited-papers.rdbu
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-proportion-of-cited-papers.sql
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-references-doi.sql
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-references-per-paper.rdbu
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-references-per-paper.sql
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-work-authors.sql
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-work-funders.sql
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-work-links.rdbu
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-work-links.sql
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-work-references.sql
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-work-subjects.sql
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly-works.sql
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/yearly_works_all.sql
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/reports/metrics.txt
+-rw-r--r--   0        0        0    19721 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/reports/subject_hierarchy.svg
+-rw-r--r--   0        0        0   400154 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/reports/subject_hierarchy.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/LICENSE
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/Makefile
+-rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/README.md
+-rwxr-xr-x   0        0        0     1899 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/create_db.sh
+-rwxr-xr-x   0        0        0     1076 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/dep2dot.sed
+-rwxr-xr-x   0        0        0      759 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/dep2tsort.sed
+-rwxr-xr-x   0        0        0     1426 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/drop_db.sh
+-rwxr-xr-x   0        0        0     3114 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/mkdep.sh
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/mktags.sh
+-rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/need_var.sh
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/psql-ctime.sql
+-rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/run_sql.sh
+-rwxr-xr-x   0        0        0     2049 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/run_test.sh
+-rwxr-xr-x   0        0        0      963 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/sync_timestamps.sh
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/.gitignore
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/Makefile
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/forked_projects.sql
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/popular_projects.sql
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/pr_projects.sql
+-rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sh
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sql
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_stars.sql
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_urls.sql
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_commit_projects.sql
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_issue_projects.sql
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/.gitignore
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/Makefile
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.rdbu
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.sql
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.rdbu
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.sql
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.rdbu
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.sql
+-rwxr-xr-x   0        0        0      457 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sh
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sql
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.rdbu
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.sql
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.rdbu
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.sql
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.rdbu
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.sql
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.rdbu
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/tables/general_field_publications
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/tables/subject_pair_fundamentalness_percentile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/tables/subject_pair_strength_percentile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/tables/work_subject_citations
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/tables/work_subject_numbers
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/unit-test/README.md
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/unit-test/subject-pair-strength-percentile.rdbu
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/graph/unit-test/work_subject_citations.svg
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/.depend
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/.depend.all
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/.gitignore
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/Makefile
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/README.md
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/citable_works.rdbu
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/citable_works.sql
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/citations.rdbu
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/citations.sql
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/impact-factor-all.rdbu
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/impact-factor-all.sql
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/impact-factor-non-review.sql
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/impact-factor-top.sql
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/impact_factor.rdbu
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/impact_factor.sql
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/impact_factor_titles.sql
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/most-cited-3y.sql
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/most-cited-in-3y.sql
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/publications.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/rolap
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/works_issn.rdbu
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/works_issn.sql
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/LICENSE
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/Makefile
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/README.md
+-rwxr-xr-x   0        0        0     1899 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/create_db.sh
+-rwxr-xr-x   0        0        0     1076 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/dep2dot.sed
+-rwxr-xr-x   0        0        0      759 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/dep2tsort.sed
+-rwxr-xr-x   0        0        0     1426 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/drop_db.sh
+-rwxr-xr-x   0        0        0     3114 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/mkdep.sh
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/mktags.sh
+-rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/need_var.sh
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/psql-ctime.sql
+-rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/run_sql.sh
+-rwxr-xr-x   0        0        0     2363 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/run_test.sh
+-rwxr-xr-x   0        0        0      963 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/sync_timestamps.sh
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/.gitignore
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/Makefile
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/forked_projects.sql
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/popular_projects.sql
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/pr_projects.sql
+-rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sh
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sql
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_stars.sql
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_urls.sql
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_commit_projects.sql
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_issue_projects.sql
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/.gitignore
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/Makefile
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.rdbu
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.sql
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.rdbu
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.sql
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.rdbu
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.sql
+-rwxr-xr-x   0        0        0      457 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sh
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sql
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.rdbu
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.sql
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.rdbu
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.sql
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.rdbu
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.sql
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.rdbu
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.sql
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/.depend
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/.depend.all
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/.gitignore
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/Makefile
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/README.md
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/issn_h5.rdbu
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/issn_h5.sql
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/journal-h5-all.sql
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/journal-h5.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/rolap
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/work_citations.rdbu
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/work_citations.sql
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/works_issn.rdbu
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/works_issn.sql
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/LICENSE
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/Makefile
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/README.md
+-rwxr-xr-x   0        0        0     1899 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/create_db.sh
+-rwxr-xr-x   0        0        0     1076 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/dep2dot.sed
+-rwxr-xr-x   0        0        0      759 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/dep2tsort.sed
+-rwxr-xr-x   0        0        0     1426 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/drop_db.sh
+-rwxr-xr-x   0        0        0     3114 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/mkdep.sh
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/mktags.sh
+-rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/need_var.sh
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/psql-ctime.sql
+-rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/run_sql.sh
+-rwxr-xr-x   0        0        0     2363 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/run_test.sh
+-rwxr-xr-x   0        0        0      963 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/sync_timestamps.sh
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/.gitignore
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/Makefile
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/forked_projects.sql
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/popular_projects.sql
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/pr_projects.sql
+-rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sh
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sql
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_stars.sql
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_urls.sql
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_commit_projects.sql
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_issue_projects.sql
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/.gitignore
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/Makefile
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.rdbu
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.sql
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.rdbu
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.sql
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.rdbu
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.sql
+-rwxr-xr-x   0        0        0      457 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sh
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sql
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.rdbu
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.sql
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.rdbu
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.sql
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.rdbu
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.sql
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.rdbu
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/journal-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.sql
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/open-access/.gitignore
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/open-access/Makefile
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/open-access/README.md
+-rwxr-xr-x   0        0        0      454 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/open-access/is-cited-by-is-normal.py
+-rwxr-xr-x   0        0        0     1674 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/open-access/oa-is-cited-more.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/open-access/oa_works.sql
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/open-access/yearly-journal-oa-work-ratio.sql
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/open-access/yearly-oa-journal-works.sql
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/orcid/.gitignore
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/orcid/Makefile
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/orcid/README.md
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/orcid/metrics.sql
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/.depend
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/.depend.all
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/.gitignore
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/Makefile
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/README.md
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/citation-graph-indexes.sql
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/citation-graph.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/orcid-h5.sql
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/orcid_h5.rdbu
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/orcid_h5.sql
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/random_other_works.sql
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/random_top_works.rdbu
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/random_top_works.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/rolap
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/work_citations.rdbu
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/work_citations.sql
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/works_orcid.rdbu
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/works_orcid.sql
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/LICENSE
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/Makefile
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/README.md
+-rwxr-xr-x   0        0        0     1899 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/create_db.sh
+-rwxr-xr-x   0        0        0     1076 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/dep2dot.sed
+-rwxr-xr-x   0        0        0      759 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/dep2tsort.sed
+-rwxr-xr-x   0        0        0     1426 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/drop_db.sh
+-rwxr-xr-x   0        0        0     3114 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/mkdep.sh
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/mktags.sh
+-rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/need_var.sh
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/psql-ctime.sql
+-rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/run_sql.sh
+-rwxr-xr-x   0        0        0     2363 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/run_test.sh
+-rwxr-xr-x   0        0        0      963 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/sync_timestamps.sh
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/.gitignore
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/Makefile
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/forked_projects.sql
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/popular_projects.sql
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/pr_projects.sql
+-rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sh
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_metrics.sql
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_stars.sql
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/project_urls.sql
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_commit_projects.sql
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/postgresql/recent_issue_projects.sql
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/.gitignore
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/Makefile
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.rdbu
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/forked_projects.sql
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.rdbu
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/popular_projects.sql
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.rdbu
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/pr_projects.sql
+-rwxr-xr-x   0        0        0      457 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sh
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_metrics.sql
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.rdbu
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_stars.sql
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.rdbu
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/project_urls.sql
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.rdbu
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_commit_projects.sql
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.rdbu
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/person-h5/simple-rolap/examples/ghtorrent-strat-sel/sqlite/recent_issue_projects.sql
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/research-synthesis/.gitignore
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/research-synthesis/Makefile
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/research-synthesis/README.md
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/research-synthesis/early-studies.sql
+-rw-r--r--   0        0        0    21448 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/research-synthesis/research-synthesis.png
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/research-synthesis/research-synthesis.sql
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/sample/.gitignore
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/sample/Makefile
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/sample/README.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/sample/indexes.sql
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/soft-eng-h5/.gitignore
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/soft-eng-h5/Makefile
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/soft-eng-h5/README.md
+-rw-r--r--   0        0        0     5915 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/soft-eng-h5/se-5y.sql
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/soft-eng-h5/venue-h5-report.sql
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/soft-eng-h5/venue_h5.sql
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/soft-eng-h5/work_citations.sql
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/soft-eng-h5/works_venue.sql
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/tawfik/.gitignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/tawfik/Makefile
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/tawfik/README.md
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/tawfik/baseline_cdindex.sql
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/tawfik/comparison-report.sql
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/tawfik/comparison.sql
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/tawfik/tawfik-works.sql
+-rw-r--r--   0        0        0    16765 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/tawfik/tawfik-works.txt
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/tawfik/tawfik_cdindex.sql
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/tawfik/tawfik_works.sql
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/yearly-numpages/.gitignore
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/yearly-numpages/Makefile
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/yearly-numpages/README.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/yearly-numpages/works_pages.rdbu
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/yearly-numpages/works_pages.sql
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/examples/yearly-numpages/yearly-numpages.sql
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/.gitignore
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/Pipfile
+-rw-r--r--   0        0        0    46118 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/Pipfile.lock
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/__init__.py
+-rwxr-xr-x   0        0        0    17839 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/__main__.py
+-rwxr-xr-x   0        0        0     5399 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/common.py
+-rw-r--r--   0        0        0    48543 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/crossref.py
+-rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/csv_sources.py
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/debug.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/file_cache.py
+-rw-r--r--   0        0        0    23397 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/orcid.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/perf.py
+-rw-r--r--   0        0        0    11882 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/ror.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/tsort.py
+-rw-r--r--   0        0        0    14968 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/virtual_db.py
+-rw-r--r--   0        0        0    16464 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/data/asjc.csv
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/sql/link-works-asjcs.sql
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/sql/normalize-asjc.sql
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/sql/normalize-doaj.sql
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/sql/normalize-journal-names-issns.sql
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/src/alexandria3k/sql/work-authors-top-rors.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/__init__.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/link-works-asjcs.rdbu
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/normalize-asjc-general-fields.rdbu
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/normalize-asjc-subject-areas.rdbu
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/normalize-asjc.rdbu
+-rwxr-xr-x   0        0        0      775 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/regression.sh
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/test_common.py
+-rw-r--r--   0        0        0    19056 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/test_crossref.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/test_csv_sources.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/test_debug.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/test_dir.py
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/test_journal_names.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/test_main.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/test_orcid.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/test_perf.py
+-rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/test_ror.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/test_tsort.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/test_virtual_db.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/work-authors-top-rors.rdbu
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/chat/chat.rdbu
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/chat/fixed.rdbu
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/chat/foo.sql
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/chat/sqlite3
+-rw-r--r--   0        0        0   115459 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/data/ORCID_2022_10_summaries.tar.gz
+-rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/data/ror.zip
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/data/titleFile.csv
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/data/sample/1item.json.gz
+-rw-r--r--   0        0        0     8634 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/data/sample/2item-references.json.gz
+-rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/data/sample/3items.json.gz
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/data/sample/affiliations.json.gz
+-rw-r--r--   0        0        0    10950 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/data/sample/funded.json.gz
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/data/sample/orcid-work.json.gz
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/data/sample/same-author.json.gz
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/data/sample/updated.json.gz
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/ref/95c37325df8acb61abe0de2dbc605c5c
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/ref/fcf9ec5d432a0bf83ed97ba390d16a32
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/tmp/README.md
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/tmp/regression/95c37325df8acb61abe0de2dbc605c5c
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/tests/tmp/regression/fcf9ec5d432a0bf83ed97ba390d16a32
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/LICENSE
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/README.md
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/pyproject.toml
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 alexandria3k-2.6.6/PKG-INFO
```

### Comparing `alexandria3k-2.6.5/.pylintrc` & `alexandria3k-2.6.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/.github/workflows/ci.yml` & `alexandria3k-2.6.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/.github/workflows/sphinx.yml` & `alexandria3k-2.6.6/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/bin/alexandria3k` & `alexandria3k-2.6.6/bin/alexandria3k`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/bin/schema2dot.sed` & `alexandria3k-2.6.6/bin/schema2dot.sed`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/bin/update-schema` & `alexandria3k-2.6.6/bin/update-schema`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/Makefile` & `alexandria3k-2.6.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/cli-eg.rst` & `alexandria3k-2.6.6/docs/cli-eg.rst`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/conf.py` & `alexandria3k-2.6.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/dev.rst` & `alexandria3k-2.6.6/docs/dev.rst`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/downloading.rst` & `alexandria3k-2.6.6/docs/downloading.rst`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/faq.rst` & `alexandria3k-2.6.6/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/index.rst` & `alexandria3k-2.6.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/installation.rst` & `alexandria3k-2.6.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/make.bat` & `alexandria3k-2.6.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/python-eg.rst` & `alexandria3k-2.6.6/docs/python-eg.rst`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/schema.rst` & `alexandria3k-2.6.6/docs/schema.rst`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/use.rst` & `alexandria3k-2.6.6/docs/use.rst`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/alexandria3k.1` & `alexandria3k-2.6.6/docs/_build/alexandria3k.1`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/.doctrees/environment.pickle` & `alexandria3k-2.6.6/docs/_build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/.doctrees/index.doctree` & `alexandria3k-2.6.6/docs/_build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/api.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/cli-eg.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/cli-eg.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/crossref.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/crossref.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/csv_sources.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/csv_sources.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/debug.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/debug.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/dev.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/dev.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/downloading.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/downloading.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/environment.pickle` & `alexandria3k-2.6.6/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/faq.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/faq.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/index.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/installation.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/orcid.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/orcid.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/perf.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/perf.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/python-eg.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/python-eg.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/ror.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/ror.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/schema.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/schema.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/use.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/use.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/doctrees/cli/index.doctree` & `alexandria3k-2.6.6/docs/_build/doctrees/cli/index.doctree`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/api.html` & `alexandria3k-2.6.6/docs/_build/html/api.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/cli-eg.html` & `alexandria3k-2.6.6/docs/_build/html/cli-eg.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/crossref.html` & `alexandria3k-2.6.6/docs/_build/html/crossref.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/csv_sources.html` & `alexandria3k-2.6.6/docs/_build/html/csv_sources.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/debug.html` & `alexandria3k-2.6.6/docs/_build/html/debug.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/dev.html` & `alexandria3k-2.6.6/docs/_build/html/dev.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/downloading.html` & `alexandria3k-2.6.6/docs/_build/html/downloading.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/faq.html` & `alexandria3k-2.6.6/docs/_build/html/faq.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/genindex.html` & `alexandria3k-2.6.6/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/index.html` & `alexandria3k-2.6.6/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/installation.html` & `alexandria3k-2.6.6/docs/_build/html/installation.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/objects.inv` & `alexandria3k-2.6.6/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/orcid.html` & `alexandria3k-2.6.6/docs/_build/html/orcid.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/perf.html` & `alexandria3k-2.6.6/docs/_build/html/perf.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/py-modindex.html` & `alexandria3k-2.6.6/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/python-eg.html` & `alexandria3k-2.6.6/docs/_build/html/python-eg.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/ror.html` & `alexandria3k-2.6.6/docs/_build/html/ror.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/schema.html` & `alexandria3k-2.6.6/docs/_build/html/schema.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/search.html` & `alexandria3k-2.6.6/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/searchindex.js` & `alexandria3k-2.6.6/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/use.html` & `alexandria3k-2.6.6/docs/_build/html/use.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_images/all.svg` & `alexandria3k-2.6.6/docs/_build/html/_images/all.svg`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_images/crossref.svg` & `alexandria3k-2.6.6/docs/_build/html/_images/crossref.svg`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_images/orcid.svg` & `alexandria3k-2.6.6/docs/_build/html/_images/orcid.svg`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_images/other.svg` & `alexandria3k-2.6.6/docs/_build/html/_images/other.svg`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_images/ror.svg` & `alexandria3k-2.6.6/docs/_build/html/_images/ror.svg`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_sources/cli-eg.rst.txt` & `alexandria3k-2.6.6/docs/_build/html/_sources/cli-eg.rst.txt`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_sources/dev.rst.txt` & `alexandria3k-2.6.6/docs/_build/html/_sources/dev.rst.txt`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_sources/downloading.rst.txt` & `alexandria3k-2.6.6/docs/_build/html/_sources/downloading.rst.txt`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_sources/faq.rst.txt` & `alexandria3k-2.6.6/docs/_build/html/_sources/faq.rst.txt`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_sources/index.rst.txt` & `alexandria3k-2.6.6/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_sources/installation.rst.txt` & `alexandria3k-2.6.6/docs/_build/html/_sources/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_sources/python-eg.rst.txt` & `alexandria3k-2.6.6/docs/_build/html/_sources/python-eg.rst.txt`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_sources/schema.rst.txt` & `alexandria3k-2.6.6/docs/_build/html/_sources/schema.rst.txt`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_sources/use.rst.txt` & `alexandria3k-2.6.6/docs/_build/html/_sources/use.rst.txt`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_static/alabaster.css` & `alexandria3k-2.6.6/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_static/basic.css` & `alexandria3k-2.6.6/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_static/doctools.js` & `alexandria3k-2.6.6/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_static/language_data.js` & `alexandria3k-2.6.6/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_static/pygments.css` & `alexandria3k-2.6.6/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_static/searchtools.js` & `alexandria3k-2.6.6/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/_static/sphinx_highlight.js` & `alexandria3k-2.6.6/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/_build/html/cli/index.html` & `alexandria3k-2.6.6/docs/_build/html/cli/index.html`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/schema/all.pdf` & `alexandria3k-2.6.6/docs/schema/all.pdf`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/schema/all.svg` & `alexandria3k-2.6.6/docs/schema/all.svg`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/schema/crossref.pdf` & `alexandria3k-2.6.6/docs/schema/crossref.pdf`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/schema/crossref.svg` & `alexandria3k-2.6.6/docs/schema/crossref.svg`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/schema/orcid.dot` & `alexandria3k-2.6.6/docs/schema/orcid.dot`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/schema/orcid.pdf` & `alexandria3k-2.6.6/docs/schema/orcid.pdf`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/schema/orcid.svg` & `alexandria3k-2.6.6/docs/schema/orcid.svg`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/schema/other.dot` & `alexandria3k-2.6.6/docs/schema/other.dot`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/schema/other.pdf` & `alexandria3k-2.6.6/docs/schema/other.pdf`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/schema/other.svg` & `alexandria3k-2.6.6/docs/schema/other.svg`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/schema/ror.dot` & `alexandria3k-2.6.6/docs/schema/ror.dot`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/schema/ror.pdf` & `alexandria3k-2.6.6/docs/schema/ror.pdf`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/docs/schema/ror.svg` & `alexandria3k-2.6.6/docs/schema/ror.svg`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/README.md` & `alexandria3k-2.6.6/examples/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 of all other studies.
 
 The following examples are available.
 
 * ["Hello world" example: number of authors by decade](authors-by-decade)
 * [Tally number of research synthesis studies](research-synthesis)
 * [Generate and study the entities' graph structure](graph)
+* [Examine the evolution and impact of open access journal papers](open-access)
 * [Report metrics associated with ORCID data](orcid)
 * [Obtain measures associated with COVID-19 research](covid)
 * [Calculate the 2021 journal impact factor](impact-factor-2021)
 * [Calculate the h5-index of journals](journal-h5)
 * [Calculate the h5-index of software engineering research venues](soft-eng-h5)
 * [Calculate h5-index of persons and study their citation graph](person-h5)
 * [Report metrics associated with the Crossref data set](crossref-standalone)
```

### Comparing `alexandria3k-2.6.5/examples/author-productivity/Makefile` & `alexandria3k-2.6.6/examples/author-productivity/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/author-productivity/README.md` & `alexandria3k-2.6.6/examples/author-productivity/README.md`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/author-productivity/frequent-names.sql` & `alexandria3k-2.6.6/examples/author-productivity/frequent-names.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/author-productivity/yearly_authors.sql` & `alexandria3k-2.6.6/examples/author-productivity/yearly_authors.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/authors-by-decade/Makefile` & `alexandria3k-2.6.6/examples/authors-by-decade/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/authors-by-decade/README.md` & `alexandria3k-2.6.6/examples/authors-by-decade/README.md`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/cdindex/Makefile` & `alexandria3k-2.6.6/examples/cdindex/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/cdindex/README.md` & `alexandria3k-2.6.6/examples/cdindex/README.md`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/cdindex/cdindex-db.cpp` & `alexandria3k-2.6.6/examples/cdindex/cdindex-db.cpp`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/cdindex/cdindex-db.py` & `alexandria3k-2.6.6/examples/cdindex/cdindex-db.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/cdindex/cdindex-otf.py` & `alexandria3k-2.6.6/examples/cdindex/cdindex-otf.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/common/Makefile` & `alexandria3k-2.6.6/examples/common/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 
 # TODO: Add rule in including Makefile to populate database with required data
 
 asjcs: populate
 	$(TIME) alexandria3k --data-source ASJC --populate "$(MAINDB).db"
 	touch $@
 
+doaj: populate
+	$(TIME) alexandria3k --data-source DOAJ --populate "$(MAINDB).db"
+	touch $@
+
 link-works-asjcs: asjcs populate
 	$(TIME) alexandria3k --execute link-works-asjcs \
 	  --populate "$(MAINDB).db"
 	touch $@
 
 rors: populate
 	$(TIME) alexandria3k --data-source ROR ../common/ror-v1.17.1-2022-12-16.zip --populate "$(MAINDB).db"
```

### Comparing `alexandria3k-2.6.5/examples/common/unit-test/works-subjects.rdbu` & `alexandria3k-2.6.6/examples/common/unit-test/works-subjects.rdbu`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/.depend.all` & `alexandria3k-2.6.6/examples/covid/.depend.all`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/author-number-quartiles.sql` & `alexandria3k-2.6.6/examples/covid/author-number-quartiles.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/inner-citations.sql` & `alexandria3k-2.6.6/examples/covid/inner-citations.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/number-of-authors.sql` & `alexandria3k-2.6.6/examples/covid/number-of-authors.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/work-affiliations.rdbu` & `alexandria3k-2.6.6/examples/covid/work-affiliations.rdbu`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/work-affiliations.sql` & `alexandria3k-2.6.6/examples/covid/work-affiliations.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/simple-rolap/LICENSE` & `alexandria3k-2.6.6/examples/covid/simple-rolap/LICENSE`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/simple-rolap/Makefile` & `alexandria3k-2.6.6/examples/covid/simple-rolap/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/simple-rolap/README.md` & `alexandria3k-2.6.6/examples/covid/simple-rolap/README.md`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/simple-rolap/create_db.sh` & `alexandria3k-2.6.6/examples/covid/simple-rolap/create_db.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/simple-rolap/dep2dot.sed` & `alexandria3k-2.6.6/examples/covid/simple-rolap/dep2dot.sed`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/simple-rolap/dep2tsort.sed` & `alexandria3k-2.6.6/examples/covid/simple-rolap/dep2tsort.sed`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/simple-rolap/drop_db.sh` & `alexandria3k-2.6.6/examples/covid/simple-rolap/drop_db.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/simple-rolap/mkdep.sh` & `alexandria3k-2.6.6/examples/covid/simple-rolap/mkdep.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/simple-rolap/mktags.sh` & `alexandria3k-2.6.6/examples/covid/simple-rolap/mktags.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/simple-rolap/need_var.sh` & `alexandria3k-2.6.6/examples/covid/simple-rolap/need_var.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/simple-rolap/psql-ctime.sql` & `alexandria3k-2.6.6/examples/covid/simple-rolap/psql-ctime.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/simple-rolap/run_sql.sh` & `alexandria3k-2.6.6/examples/covid/simple-rolap/run_sql.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/simple-rolap/run_test.sh` & `alexandria3k-2.6.6/examples/covid/simple-rolap/run_test.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/covid/simple-rolap/sync_timestamps.sh` & `alexandria3k-2.6.6/examples/covid/simple-rolap/sync_timestamps.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/crossref-standalone/Makefile` & `alexandria3k-2.6.6/examples/crossref-standalone/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/cs_cdindex/Makefile` & `alexandria3k-2.6.6/examples/cs_cdindex/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/cs_cdindex/cdindex-by-type.sql` & `alexandria3k-2.6.6/examples/cs_cdindex/cdindex-by-type.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/cs_cdindex/cs_works.sed` & `alexandria3k-2.6.6/examples/cs_cdindex/cs_works.sed`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/cs_cdindex/top-consolidating.sql` & `alexandria3k-2.6.6/examples/cs_cdindex/top-consolidating.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/cs_cdindex/top-disruptive.sql` & `alexandria3k-2.6.6/examples/cs_cdindex/top-disruptive.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/.depend` & `alexandria3k-2.6.6/examples/graph/.depend`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/.depend.all` & `alexandria3k-2.6.6/examples/graph/.depend.all`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/Makefile` & `alexandria3k-2.6.6/examples/graph/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/README.md` & `alexandria3k-2.6.6/examples/graph/README.md`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/author-number-quartiles-2020.sql` & `alexandria3k-2.6.6/examples/graph/author-number-quartiles-2020.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/author-number-quartiles-medicine-2020.sql` & `alexandria3k-2.6.6/examples/graph/author-number-quartiles-medicine-2020.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/author-number-quartiles-medicine.sql` & `alexandria3k-2.6.6/examples/graph/author-number-quartiles-medicine.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/author-number-quartiles.sql` & `alexandria3k-2.6.6/examples/graph/author-number-quartiles.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/fields_by_year.svg` & `alexandria3k-2.6.6/examples/graph/fields_by_year.svg`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/general-field-publications-list.sql` & `alexandria3k-2.6.6/examples/graph/general-field-publications-list.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/general_field_publications.sql` & `alexandria3k-2.6.6/examples/graph/general_field_publications.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/graph.dot` & `alexandria3k-2.6.6/examples/graph/graph.dot`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/graph.png` & `alexandria3k-2.6.6/examples/graph/graph.png`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/metrics.sql` & `alexandria3k-2.6.6/examples/graph/metrics.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/subject_hierarchy.sql` & `alexandria3k-2.6.6/examples/graph/subject_hierarchy.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/subject_hierarchy.svg` & `alexandria3k-2.6.6/examples/graph/subject_hierarchy.svg`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/subject_pair_fundamentalness_percentile.sql` & `alexandria3k-2.6.6/examples/graph/subject_pair_fundamentalness_percentile.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/subject_pair_strength_percentile.sql` & `alexandria3k-2.6.6/examples/graph/subject_pair_strength_percentile.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/twenty_year_citations.sql` & `alexandria3k-2.6.6/examples/graph/twenty_year_citations.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/twenty_year_publications.rdbu` & `alexandria3k-2.6.6/examples/graph/twenty_year_publications.rdbu`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/two_year_citations.sql` & `alexandria3k-2.6.6/examples/graph/two_year_citations.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/work_subject_citations.sql` & `alexandria3k-2.6.6/examples/graph/work_subject_citations.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/yearly-author-affiliations.sql` & `alexandria3k-2.6.6/examples/graph/yearly-author-affiliations.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/yearly-citations-per-paper.sql` & `alexandria3k-2.6.6/examples/graph/yearly-citations-per-paper.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/yearly-funder-awards.sql` & `alexandria3k-2.6.6/examples/graph/yearly-funder-awards.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/yearly-proportion-of-cited-papers.sql` & `alexandria3k-2.6.6/examples/graph/yearly-proportion-of-cited-papers.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/yearly-references-per-paper.sql` & `alexandria3k-2.6.6/examples/graph/yearly-references-per-paper.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/reports/subject_hierarchy.svg` & `alexandria3k-2.6.6/examples/graph/reports/subject_hierarchy.svg`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/reports/subject_hierarchy.txt` & `alexandria3k-2.6.6/examples/graph/reports/subject_hierarchy.txt`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/simple-rolap/LICENSE` & `alexandria3k-2.6.6/examples/graph/simple-rolap/LICENSE`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/simple-rolap/Makefile` & `alexandria3k-2.6.6/examples/graph/simple-rolap/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/simple-rolap/README.md` & `alexandria3k-2.6.6/examples/graph/simple-rolap/README.md`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/simple-rolap/create_db.sh` & `alexandria3k-2.6.6/examples/graph/simple-rolap/create_db.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/simple-rolap/dep2dot.sed` & `alexandria3k-2.6.6/examples/graph/simple-rolap/dep2dot.sed`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/simple-rolap/dep2tsort.sed` & `alexandria3k-2.6.6/examples/graph/simple-rolap/dep2tsort.sed`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/simple-rolap/drop_db.sh` & `alexandria3k-2.6.6/examples/graph/simple-rolap/drop_db.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/simple-rolap/mkdep.sh` & `alexandria3k-2.6.6/examples/graph/simple-rolap/mkdep.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/simple-rolap/mktags.sh` & `alexandria3k-2.6.6/examples/graph/simple-rolap/mktags.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/simple-rolap/need_var.sh` & `alexandria3k-2.6.6/examples/graph/simple-rolap/need_var.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/simple-rolap/psql-ctime.sql` & `alexandria3k-2.6.6/examples/graph/simple-rolap/psql-ctime.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/simple-rolap/run_sql.sh` & `alexandria3k-2.6.6/examples/graph/simple-rolap/run_sql.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/simple-rolap/run_test.sh` & `alexandria3k-2.6.6/examples/graph/simple-rolap/run_test.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/simple-rolap/sync_timestamps.sh` & `alexandria3k-2.6.6/examples/graph/simple-rolap/sync_timestamps.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/unit-test/subject-pair-strength-percentile.rdbu` & `alexandria3k-2.6.6/examples/graph/unit-test/subject-pair-strength-percentile.rdbu`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/graph/unit-test/work_subject_citations.svg` & `alexandria3k-2.6.6/examples/graph/unit-test/work_subject_citations.svg`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/.depend.all` & `alexandria3k-2.6.6/examples/impact-factor-2021/.depend.all`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/Makefile` & `alexandria3k-2.6.6/examples/impact-factor-2021/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/citations.sql` & `alexandria3k-2.6.6/examples/impact-factor-2021/citations.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/impact-factor-all.sql` & `alexandria3k-2.6.6/examples/impact-factor-2021/impact-factor-all.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/impact_factor_titles.sql` & `alexandria3k-2.6.6/examples/impact-factor-2021/impact_factor_titles.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/LICENSE` & `alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/LICENSE`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/Makefile` & `alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/README.md` & `alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/README.md`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/create_db.sh` & `alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/create_db.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/dep2dot.sed` & `alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/dep2dot.sed`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/dep2tsort.sed` & `alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/dep2tsort.sed`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/drop_db.sh` & `alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/drop_db.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/mkdep.sh` & `alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/mkdep.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/mktags.sh` & `alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/mktags.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/need_var.sh` & `alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/need_var.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/psql-ctime.sql` & `alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/psql-ctime.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/run_sql.sh` & `alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/run_sql.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/run_test.sh` & `alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/run_test.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/impact-factor-2021/simple-rolap/sync_timestamps.sh` & `alexandria3k-2.6.6/examples/impact-factor-2021/simple-rolap/sync_timestamps.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/Makefile` & `alexandria3k-2.6.6/examples/journal-h5/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/README.md` & `alexandria3k-2.6.6/examples/journal-h5/README.md`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/issn_h5.sql` & `alexandria3k-2.6.6/examples/journal-h5/issn_h5.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/journal-h5-all.sql` & `alexandria3k-2.6.6/examples/journal-h5/journal-h5-all.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/journal-h5.sql` & `alexandria3k-2.6.6/examples/journal-h5/journal-h5.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/simple-rolap/LICENSE` & `alexandria3k-2.6.6/examples/journal-h5/simple-rolap/LICENSE`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/simple-rolap/Makefile` & `alexandria3k-2.6.6/examples/journal-h5/simple-rolap/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/simple-rolap/README.md` & `alexandria3k-2.6.6/examples/journal-h5/simple-rolap/README.md`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/simple-rolap/create_db.sh` & `alexandria3k-2.6.6/examples/journal-h5/simple-rolap/create_db.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/simple-rolap/dep2dot.sed` & `alexandria3k-2.6.6/examples/journal-h5/simple-rolap/dep2dot.sed`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/simple-rolap/dep2tsort.sed` & `alexandria3k-2.6.6/examples/journal-h5/simple-rolap/dep2tsort.sed`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/simple-rolap/drop_db.sh` & `alexandria3k-2.6.6/examples/journal-h5/simple-rolap/drop_db.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/simple-rolap/mkdep.sh` & `alexandria3k-2.6.6/examples/journal-h5/simple-rolap/mkdep.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/simple-rolap/mktags.sh` & `alexandria3k-2.6.6/examples/journal-h5/simple-rolap/mktags.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/simple-rolap/need_var.sh` & `alexandria3k-2.6.6/examples/journal-h5/simple-rolap/need_var.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/simple-rolap/psql-ctime.sql` & `alexandria3k-2.6.6/examples/journal-h5/simple-rolap/psql-ctime.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/simple-rolap/run_sql.sh` & `alexandria3k-2.6.6/examples/journal-h5/simple-rolap/run_sql.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/simple-rolap/run_test.sh` & `alexandria3k-2.6.6/examples/journal-h5/simple-rolap/run_test.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/journal-h5/simple-rolap/sync_timestamps.sh` & `alexandria3k-2.6.6/examples/journal-h5/simple-rolap/sync_timestamps.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/orcid/metrics.sql` & `alexandria3k-2.6.6/examples/orcid/metrics.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/.depend.all` & `alexandria3k-2.6.6/examples/person-h5/.depend.all`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/Makefile` & `alexandria3k-2.6.6/examples/person-h5/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/citation-graph.py` & `alexandria3k-2.6.6/examples/person-h5/citation-graph.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/orcid_h5.sql` & `alexandria3k-2.6.6/examples/person-h5/orcid_h5.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/random_other_works.sql` & `alexandria3k-2.6.6/examples/person-h5/random_other_works.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/random_top_works.rdbu` & `alexandria3k-2.6.6/examples/person-h5/random_top_works.rdbu`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/random_top_works.sql` & `alexandria3k-2.6.6/examples/person-h5/random_top_works.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/simple-rolap/LICENSE` & `alexandria3k-2.6.6/examples/person-h5/simple-rolap/LICENSE`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/simple-rolap/Makefile` & `alexandria3k-2.6.6/examples/person-h5/simple-rolap/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/simple-rolap/README.md` & `alexandria3k-2.6.6/examples/person-h5/simple-rolap/README.md`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/simple-rolap/create_db.sh` & `alexandria3k-2.6.6/examples/person-h5/simple-rolap/create_db.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/simple-rolap/dep2dot.sed` & `alexandria3k-2.6.6/examples/person-h5/simple-rolap/dep2dot.sed`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/simple-rolap/dep2tsort.sed` & `alexandria3k-2.6.6/examples/person-h5/simple-rolap/dep2tsort.sed`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/simple-rolap/drop_db.sh` & `alexandria3k-2.6.6/examples/person-h5/simple-rolap/drop_db.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/simple-rolap/mkdep.sh` & `alexandria3k-2.6.6/examples/person-h5/simple-rolap/mkdep.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/simple-rolap/mktags.sh` & `alexandria3k-2.6.6/examples/person-h5/simple-rolap/mktags.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/simple-rolap/need_var.sh` & `alexandria3k-2.6.6/examples/person-h5/simple-rolap/need_var.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/simple-rolap/psql-ctime.sql` & `alexandria3k-2.6.6/examples/person-h5/simple-rolap/psql-ctime.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/simple-rolap/run_sql.sh` & `alexandria3k-2.6.6/examples/person-h5/simple-rolap/run_sql.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/simple-rolap/run_test.sh` & `alexandria3k-2.6.6/examples/person-h5/simple-rolap/run_test.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/person-h5/simple-rolap/sync_timestamps.sh` & `alexandria3k-2.6.6/examples/person-h5/simple-rolap/sync_timestamps.sh`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/research-synthesis/Makefile` & `alexandria3k-2.6.6/examples/research-synthesis/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/research-synthesis/early-studies.sql` & `alexandria3k-2.6.6/examples/research-synthesis/early-studies.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/research-synthesis/research-synthesis.png` & `alexandria3k-2.6.6/examples/research-synthesis/research-synthesis.png`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/research-synthesis/research-synthesis.sql` & `alexandria3k-2.6.6/examples/research-synthesis/research-synthesis.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/sample/indexes.sql` & `alexandria3k-2.6.6/examples/sample/indexes.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/soft-eng-h5/Makefile` & `alexandria3k-2.6.6/examples/soft-eng-h5/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/soft-eng-h5/se-5y.sql` & `alexandria3k-2.6.6/examples/soft-eng-h5/se-5y.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/soft-eng-h5/venue_h5.sql` & `alexandria3k-2.6.6/examples/soft-eng-h5/venue_h5.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/soft-eng-h5/works_venue.sql` & `alexandria3k-2.6.6/examples/soft-eng-h5/works_venue.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/tawfik/Makefile` & `alexandria3k-2.6.6/examples/tawfik/Makefile`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/tawfik/README.md` & `alexandria3k-2.6.6/examples/tawfik/README.md`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/tawfik/baseline_cdindex.sql` & `alexandria3k-2.6.6/examples/tawfik/baseline_cdindex.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/tawfik/comparison.sql` & `alexandria3k-2.6.6/examples/tawfik/comparison.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/examples/tawfik/tawfik-works.txt` & `alexandria3k-2.6.6/examples/tawfik/tawfik-works.txt`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/__main__.py` & `alexandria3k-2.6.6/src/alexandria3k/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import sqlite3
 import sys
 
 from alexandria3k import crossref
 from alexandria3k import csv_sources
 from alexandria3k import debug
 from alexandria3k.file_cache import FileCache
+from alexandria3k.common import program_version
 from alexandria3k import orcid
 from alexandria3k import ror
 from alexandria3k import perf
 
 DESCRIPTION = "alexandria3k: Relational interface to publication metadata"
 
 # Default values for diverse data sources
@@ -312,14 +313,20 @@
         "--sample",
         # By default the function always returns True
         default="True",
         type=str,
         help="Python expression to sample the Crossref tables (e.g. random.random() < 0.0002)",
     )
     parser.add_argument(
+        "-v",
+        "--version",
+        action="store_true",
+        help="Report program version and exit",
+    )
+    parser.add_argument(
         "-x",
         "--execute",
         type=str,
         help="""Operation to execute on the data. This can be one of:
 link-aa-base-ror (link author affiliations to base-level research
 organizations);
 link-aa-top-ror (link author affiliations to top-level research organizations);
@@ -423,14 +430,18 @@
         debug.set_output(sys.stderr)
     perf.log("Start")
 
     if args.list_schema:
         schema_list(parser, args.list_schema)
         sys.exit(0)
 
+    if args.version:
+        print(f"alexandria3k version {program_version()}")
+        sys.exit(0)
+
     crossref_instance = None
     if args.crossref:
         # pylint: disable-next=W0123
         sample = eval(f"lambda path: {args.sample}")
         crossref_instance = crossref.Crossref(
             args.crossref, sample, args.attach_databases
         )
```

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/common.py` & `alexandria3k-2.6.6/src/alexandria3k/common.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/crossref.py` & `alexandria3k-2.6.6/src/alexandria3k/crossref.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/csv_sources.py` & `alexandria3k-2.6.6/src/alexandria3k/csv_sources.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/debug.py` & `alexandria3k-2.6.6/src/alexandria3k/debug.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/file_cache.py` & `alexandria3k-2.6.6/src/alexandria3k/file_cache.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/orcid.py` & `alexandria3k-2.6.6/src/alexandria3k/orcid.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/perf.py` & `alexandria3k-2.6.6/src/alexandria3k/perf.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/ror.py` & `alexandria3k-2.6.6/src/alexandria3k/ror.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/tsort.py` & `alexandria3k-2.6.6/src/alexandria3k/tsort.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/virtual_db.py` & `alexandria3k-2.6.6/src/alexandria3k/virtual_db.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/data/asjc.csv` & `alexandria3k-2.6.6/src/alexandria3k/data/asjc.csv`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/sql/link-works-asjcs.sql` & `alexandria3k-2.6.6/src/alexandria3k/sql/link-works-asjcs.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/sql/normalize-asjc.sql` & `alexandria3k-2.6.6/src/alexandria3k/sql/normalize-asjc.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/sql/normalize-doaj.sql` & `alexandria3k-2.6.6/src/alexandria3k/sql/normalize-doaj.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/sql/normalize-journal-names-issns.sql` & `alexandria3k-2.6.6/src/alexandria3k/sql/normalize-journal-names-issns.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k/sql/work-authors-top-rors.sql` & `alexandria3k-2.6.6/src/alexandria3k/sql/work-authors-top-rors.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k-2.6.4.dist-info/METADATA` & `alexandria3k-2.6.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alexandria3k
-Version: 2.6.4
+Version: 2.6.6
 Summary: Efficient relational database queries over the entire Crossref abnd ORCID data sets
 Project-URL: Homepage, https://github.com/dspinellis/alexandria3k
 Project-URL: Bug Tracker, https://github.com/dspinellis/alexandria3k/issues
 Author-email: Diomidis Spinellis <dds@aueb.gr>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/alexandria3k-2.6.4.dist-info/licenses/LICENSE` & `alexandria3k-2.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/foo/lib/python3.9/site-packages/pip/_vendor/chardet/euctwprober.py` & `alexandria3k-2.6.6/tests/test_perf.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-######################## BEGIN LICENSE BLOCK ########################
-# The Original Code is mozilla.org code.
 #
-# The Initial Developer of the Original Code is
-# Netscape Communications Corporation.
-# Portions created by the Initial Developer are Copyright (C) 1998
-# the Initial Developer. All Rights Reserved.
+# Alexandria3k Crossref bibliographic metadata processing
+# Copyright (C) 2022  Diomidis Spinellis
+# SPDX-License-Identifier: GPL-3.0-or-later
 #
-# Contributor(s):
-#   Mark Pilgrim - port to Python
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
 #
-# This library is free software; you can redistribute it and/or
-# modify it under the terms of the GNU Lesser General Public
-# License as published by the Free Software Foundation; either
-# version 2.1 of the License, or (at your option) any later version.
-#
-# This library is distributed in the hope that it will be useful,
+# This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# Lesser General Public License for more details.
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
-# You should have received a copy of the GNU Lesser General Public
-# License along with this library; if not, write to the Free Software
-# Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA
-# 02110-1301  USA
-######################### END LICENSE BLOCK #########################
-
-from .mbcharsetprober import MultiByteCharSetProber
-from .codingstatemachine import CodingStateMachine
-from .chardistribution import EUCTWDistributionAnalysis
-from .mbcssm import EUCTW_SM_MODEL
-
-class EUCTWProber(MultiByteCharSetProber):
-    def __init__(self):
-        super(EUCTWProber, self).__init__()
-        self.coding_sm = CodingStateMachine(EUCTW_SM_MODEL)
-        self.distribution_analyzer = EUCTWDistributionAnalysis()
-        self.reset()
-
-    @property
-    def charset_name(self):
-        return "EUC-TW"
-
-    @property
-    def language(self):
-        return "Taiwan"
+"""Performance module test"""
+
+import io
+import sys
+import unittest
+
+from .test_dir import add_src_dir
+add_src_dir()
+
+from alexandria3k import debug
+from alexandria3k import perf
+
+
+class TestPerf(unittest.TestCase):
+    def test_no_output(self):
+
+        f = io.StringIO()
+        debug.set_output(f)
+
+        perf.log("One message")
+        self.assertRegex(f.getvalue(), r"^$")
+
+    def test_output(self):
+
+        debug.set_flags(["perf"])
+        f = io.StringIO()
+        debug.set_output(f)
+
+        perf.log("phase 1")
+        self.assertRegex(f.getvalue(), r"phase 1")
```

### Comparing `alexandria3k-2.6.5/src/Pipfile.lock` & `alexandria3k-2.6.6/src/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/src/alexandria3k/perf.py` & `alexandria3k-2.6.6/tests/normalize-asjc-general-fields.rdbu`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
 # Alexandria3k Crossref bibliographic metadata processing
-# Copyright (C) 2022-2023  Diomidis Spinellis
+# Copyright (C) 2022  Diomidis Spinellis
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -12,47 +12,29 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
-"""Maintain and output time performance values."""
-
-import time
-
-from alexandria3k import debug
-
-PERF_FLAG = "perf"
-
-# By default use perf_counter() rather than process_time() to also
-# take into account I/O time
-counter = time.perf_counter
-start = counter()
-previous = start
-
-
-def log(message):
-    """Print the specified performance message and times.
-    This will output the relative elapsed time from the previous
-    output, the absolute time since the program's start, and
-    the specified message.
-
-    To obtain performance output messages you need to enable the
-    corresponding debug flag.
-
-    .. code-block:: python
+# rdbunit test for normalizing ASJC contents
+#
 
-        debug.enable_flags(["perf"]).
+BEGIN SETUP
+asjc_import:
+id	field			subject_area
+1000	Multidisciplinary	Multidisciplinary
+1100	"General Agricultural"	"Life Sciences"
+1101	"Biological Sciences"	"Life Sciences"
+1102	"Agronomy"		"Life Sciences"
+
+END
+
+INCLUDE CREATE src/alexandria3k/sql/normalize-asjc.sql
+
+BEGIN RESULT
+asjc_general_fields:
+id	name
+1000	Multidisciplinary
+1100	Agricultural
 
-    :param message: Message to output
-    :type message: str
-    """
-    if not debug.enabled(PERF_FLAG):
-        return
-    now = counter()
-    relative = now - start
-    # pylint: disable-next=invalid-name,global-statement
-    global previous
-    delta = now - previous
-    debug.log(PERF_FLAG, f"{relative:10} {delta:10} {message}")
-    previous = now
+END
```

### Comparing `alexandria3k-2.6.5/tests/link-works-asjcs.rdbu` & `alexandria3k-2.6.6/tests/link-works-asjcs.rdbu`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/normalize-asjc-general-fields.rdbu` & `alexandria3k-2.6.6/tests/normalize-asjc-subject-areas.rdbu`

 * *Files 4% similar despite different names*

```diff
@@ -28,13 +28,13 @@
 1102	"Agronomy"		"Life Sciences"
 
 END
 
 INCLUDE CREATE src/alexandria3k/sql/normalize-asjc.sql
 
 BEGIN RESULT
-asjc_general_fields:
+asjc_subject_areas:
 id	name
-1000	Multidisciplinary
-1100	Agricultural
+1	"Life Sciences"
+2	Multidisciplinary
 
 END
```

### Comparing `alexandria3k-2.6.5/tests/normalize-asjc-subject-areas.rdbu` & `alexandria3k-2.6.6/tests/normalize-asjc.rdbu`

 * *Files 12% similar despite different names*

```diff
@@ -28,13 +28,15 @@
 1102	"Agronomy"		"Life Sciences"
 
 END
 
 INCLUDE CREATE src/alexandria3k/sql/normalize-asjc.sql
 
 BEGIN RESULT
-asjc_subject_areas:
-id	name
-1	"Life Sciences"
-2	Multidisciplinary
+asjcs:
+id	field			subject_area_id		general_field_id
+1000	Multidisciplinary	2			1000
+1100	"General Agricultural"	1			1100
+1101	"Biological Sciences"	1			1100
+1102	"Agronomy"		1			1100
 
 END
```

### Comparing `alexandria3k-2.6.5/tests/test_common.py` & `alexandria3k-2.6.6/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/test_crossref.py` & `alexandria3k-2.6.6/tests/test_crossref.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/test_csv_sources.py` & `alexandria3k-2.6.6/tests/test_csv_sources.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/test_debug.py` & `alexandria3k-2.6.6/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/test_dir.py` & `alexandria3k-2.6.6/tests/test_dir.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/test_journal_names.py` & `alexandria3k-2.6.6/tests/test_journal_names.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/test_main.py` & `alexandria3k-2.6.6/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/test_orcid.py` & `alexandria3k-2.6.6/tests/test_orcid.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/test_ror.py` & `alexandria3k-2.6.6/tests/test_ror.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/test_tsort.py` & `alexandria3k-2.6.6/tests/test_tsort.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/test_virtual_db.py` & `alexandria3k-2.6.6/tests/test_virtual_db.py`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/work-authors-top-rors.rdbu` & `alexandria3k-2.6.6/tests/work-authors-top-rors.rdbu`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/chat/fixed.rdbu` & `alexandria3k-2.6.6/tests/chat/fixed.rdbu`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/chat/foo.sql` & `alexandria3k-2.6.6/tests/chat/foo.sql`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/chat/sqlite3` & `alexandria3k-2.6.6/tests/chat/sqlite3`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/data/ORCID_2022_10_summaries.tar.gz` & `alexandria3k-2.6.6/tests/data/ORCID_2022_10_summaries.tar.gz`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/data/ror.zip` & `alexandria3k-2.6.6/tests/data/ror.zip`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/data/titleFile.csv` & `alexandria3k-2.6.6/tests/data/titleFile.csv`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/data/sample/1item.json.gz` & `alexandria3k-2.6.6/tests/data/sample/1item.json.gz`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/data/sample/2item-references.json.gz` & `alexandria3k-2.6.6/tests/data/sample/2item-references.json.gz`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/data/sample/3items.json.gz` & `alexandria3k-2.6.6/tests/data/sample/3items.json.gz`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/data/sample/affiliations.json.gz` & `alexandria3k-2.6.6/tests/data/sample/affiliations.json.gz`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/data/sample/funded.json.gz` & `alexandria3k-2.6.6/tests/data/sample/funded.json.gz`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/data/sample/orcid-work.json.gz` & `alexandria3k-2.6.6/tests/data/sample/orcid-work.json.gz`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/data/sample/same-author.json.gz` & `alexandria3k-2.6.6/tests/data/sample/same-author.json.gz`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/tests/data/sample/updated.json.gz` & `alexandria3k-2.6.6/tests/data/sample/updated.json.gz`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/README.md` & `alexandria3k-2.6.6/README.md`

 * *Files identical despite different names*

### Comparing `alexandria3k-2.6.5/pyproject.toml` & `alexandria3k-2.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "alexandria3k"
-version = "2.6.5"
+version = "2.6.6"
 authors = [
   { name="Diomidis Spinellis", email="dds@aueb.gr" },
 ]
 description = "Efficient relational database queries over the entire Crossref abnd ORCID data sets"
 readme = "README.md"
 requires-python = ">=3.7"
```

