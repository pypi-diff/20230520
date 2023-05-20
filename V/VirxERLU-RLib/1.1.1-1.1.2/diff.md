# Comparing `tmp/VirxERLU_RLib-1.1.1.tar.gz` & `tmp/VirxERLU_RLib-1.1.2.tar.gz`

## Comparing `VirxERLU_RLib-1.1.1.tar` & `VirxERLU_RLib-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 VirxERLU_RLib-1.1.1/Cargo.toml
--rw-r--r--   0     1001      123     3406 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/README.md
--rw-r--r--   0     1001      123      597 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/pyproject.toml
--rw-r--r--   0     1001      123     8401 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/air.rs
--rw-r--r--   0     1001      123    11816 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/analyzer.rs
--rw-r--r--   0     1001      123    18567 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/car.rs
--rw-r--r--   0     1001      123     2956 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/constants.rs
--rw-r--r--   0     1001      123     7690 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/ground.rs
--rw-r--r--   0     1001      123    19062 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/lib.rs
--rw-r--r--   0     1001      123    10689 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/pytypes.rs
--rw-r--r--   0     1001      123     8610 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/shot.rs
--rw-r--r--   0     1001      123     6345 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/src/utils.rs
--rw-r--r--   0     1001      123     4764 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/virx_erlu_rlib.pyi
--rw-r--r--   0     1001      123    12715 2023-05-10 04:08:49.000000 VirxERLU_RLib-1.1.1/Cargo.lock
--rw-r--r--   0        0        0     4211 1970-01-01 00:00:00.000000 VirxERLU_RLib-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 VirxERLU_RLib-1.1.2/Cargo.toml
+-rw-r--r--   0     1001      123    12715 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/Cargo.lock
+-rw-r--r--   0     1001      123     3406 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/README.md
+-rw-r--r--   0     1001      123      597 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/pyproject.toml
+-rw-r--r--   0     1001      123     8684 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/air.rs
+-rw-r--r--   0     1001      123    12054 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/analyzer.rs
+-rw-r--r--   0     1001      123    20096 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/car.rs
+-rw-r--r--   0     1001      123     2956 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/constants.rs
+-rw-r--r--   0     1001      123     7931 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/ground.rs
+-rw-r--r--   0     1001      123    19188 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/lib.rs
+-rw-r--r--   0     1001      123    10833 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/pytypes.rs
+-rw-r--r--   0     1001      123     8713 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/shot.rs
+-rw-r--r--   0     1001      123     5677 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/src/utils.rs
+-rw-r--r--   0     1001      123     4764 2023-05-20 05:42:46.000000 VirxERLU_RLib-1.1.2/virx_erlu_rlib.pyi
+-rw-r--r--   0        0        0     4211 1970-01-01 00:00:00.000000 VirxERLU_RLib-1.1.2/PKG-INFO
```

### Comparing `VirxERLU_RLib-1.1.1/Cargo.toml` & `VirxERLU_RLib-1.1.2/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 [package]
 name = "virx_erlu_rlib"
-version = "1.1.1"
+version = "1.1.2"
 edition = "2021"
 authors = ["VirxEC <virx@virxcase.dev>"]
 readme = "README.md"
 description = "Rust modules for VirxERLU"
 homepage = "https://github.com/VirxEC/VirxERLU-RLib"
 license = "MIT"
 include = ["/src", "pyproject.toml", "virx_erlu_rlib.pyi", "/README.md"]
 publish = false
 rust-version = "1.65"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 name = "virx_erlu_rlib"
-crate-type = ["cdylib"]
+crate-type = ["cdylib", "rlib"]
 path = "src/lib.rs"
 
 [dependencies]
-dubins_paths = { version = "1.6.0", features = ["glam"] }
+dubins_paths = { version = "1.7.0", features = ["glam"] }
 combo_vec = "0.5.1"
 
+[dev-dependencies]
+rand = "0.8.5"
+
 [dependencies.rl_ball_sym]
 version = "3.0.0"
 default-features = false
 features = ["stable-compression", "standard", "dropshot", "hoops", "throwback"]
 
 [dependencies.glam]
 version = "0.24.0"
 features = ["fast-math"]
 
 [dependencies.pyo3]
 version = "0.18.1"
-features = ["extension-module", "abi3-py37"]
+features = ["abi3-py37"]
 
-[dev-dependencies]
-rand = "0.8"
+[features]
+default = ["pyo3/extension-module"]
 
 [profile.release]
 codegen-units = 1
 panic = "abort"
 lto = true
 strip = true
+
+[profile.release-with-debug]
+inherits = "release"
+strip = false
+debug = true
```

### Comparing `VirxERLU_RLib-1.1.1/README.md` & `VirxERLU_RLib-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `VirxERLU_RLib-1.1.1/pyproject.toml` & `VirxERLU_RLib-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `VirxERLU_RLib-1.1.1/src/air.rs` & `VirxERLU_RLib-1.1.2/src/air.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use std::f32::consts::PI;
 
 use dubins_paths::{NoPathError, Result as DubinsResult};
 use glam::Vec3A;
 
 use crate::{
-    car::Car,
+    car::{Car, State},
     constants::*,
     pytypes::{BasicShotInfo, ShotType},
     BoostAmount, Mutators,
 };
 
 #[inline]
 fn angle_3d(a: Vec3A, b: Vec3A) -> f32 {
@@ -21,20 +21,22 @@
     pub jump_type: AerialJumpType,
     pub final_target: Vec3A,
     pub wait_for_land: bool,
 }
 
 impl AerialTargetInfo {
     #[inline]
+    #[must_use]
     pub const fn get_basic_shot_info(&self, time: f32) -> BasicShotInfo {
         BasicShotInfo::found(time, ShotType::Aerial, self.shot_vector, true, self.wait_for_land)
     }
 }
 
 /// Estimation of if a pre-established aerial shot is still possible
+#[must_use]
 pub fn partial_validate(target: Vec3A, xf: Vec3A, vf: Vec3A, boost_amount: BoostAmount, boost_accel: f32, car_boost: f32, time_remaining: f32) -> bool {
     let delta_x = target - xf;
     let Some(f) = delta_x.try_normalize() else {
         return true;
     };
 
     let required_acc = delta_x.length() / time_remaining.powi(2);
@@ -114,21 +116,21 @@
     mutators: Mutators,
     gravity: Vec3A,
     target: Vec3A,
     shot_vector: Vec3A,
     time_remaining: f32,
     check_target_angle: Option<Vec3A>,
 ) -> DubinsResult<AerialTargetInfo> {
-    let is_on_ground = !car.airborne || time_remaining > car.time_to_land;
+    let is_on_ground = car.car_state == State::Grounded || time_remaining > car.time_to_land;
 
-    if is_on_ground && car.up.z >= 0. && time_remaining <= JUMP_MAX_DURATION {
+    if is_on_ground && car.rotmat.z_axis.z >= 0. && time_remaining <= JUMP_MAX_DURATION {
         return Err(NoPathError);
     }
 
-    let land_time = if car.airborne { car.time_to_land } else { car.last_landing_time };
+    let land_time = if car.car_state != State::Grounded { car.time_to_land } else { car.last_landing_time };
     if is_on_ground && land_time + ON_GROUND_WAIT_TIME > time_remaining {
         return Err(NoPathError);
     }
 
     let quick_speed_required = car.location.distance(target) / time_remaining;
     if quick_speed_required > MAX_SPEED {
         return Err(NoPathError);
@@ -150,72 +152,76 @@
         |car_location: Vec3A| check_target_angle.map_or(true, |ball_location| angle_3d((car_location - ball_location).normalize(), -shot_vector) < PI / 2.);
 
     let ground_time_remaining = time_remaining - car.time_to_land - car.wait_to_jump_time;
     if is_on_ground && ground_time_remaining > 0. && target_angle_check(car.landing_location) {
         const TOTAL_JUMP_ACC: f32 = JUMP_SPEED + JUMP_ACC * JUMP_MAX_DURATION;
 
         let basic_aerial_info = BasicAerialInfo {
-            car_forward: car.landing_forward,
+            car_forward: car.landing_rotmat.x_axis,
             car_boost: f32::from(car.boost),
             boost_amount: mutators.boost_amount,
             boost_accel,
             target,
             time_remaining: ground_time_remaining,
             // car,
         };
 
         if time_remaining > DOUBLE_JUMP_DURATION {
             const TOTAL_JUMP_ACC_2: f32 = JUMP_SPEED + TOTAL_JUMP_ACC;
             const PARITAL_JUMP_LOC: f32 = 2. * JUMP_SPEED + JUMP_ACC * JUMP_MAX_DURATION;
             const JUMP_LOC_P2: f32 = -(JUMP_SPEED * JUMP_MAX_DURATION + 0.5 * JUMP_MAX_DURATION * JUMP_MAX_DURATION * JUMP_ACC);
 
-            let vf = vf_base + car.up * TOTAL_JUMP_ACC_2;
-            let xf = car.landing_location + xf_base + car.up * (time_remaining * PARITAL_JUMP_LOC + JUMP_LOC_P2);
+            let vf = vf_base + car.rotmat.z_axis * TOTAL_JUMP_ACC_2;
+            let xf = car.landing_location + xf_base + car.rotmat.z_axis * (time_remaining * PARITAL_JUMP_LOC + JUMP_LOC_P2);
 
             if let Some((jump_type, boost)) = basic_aerial_info.validate(xf, vf, AerialJumpType::Double) {
                 found.push((jump_type, boost, true));
             }
         }
 
         if time_remaining > JUMP_MAX_DURATION {
             const PARITAL_JUMP_LOC: f32 = JUMP_SPEED + JUMP_ACC * JUMP_MAX_DURATION;
             const JUMP_LOC_P2: f32 = -0.5 * JUMP_MAX_DURATION * JUMP_MAX_DURATION * JUMP_ACC;
 
-            let vf = vf_base + car.up * TOTAL_JUMP_ACC;
-            let xf = car.landing_location + xf_base + car.up * (time_remaining * PARITAL_JUMP_LOC + JUMP_LOC_P2);
+            let vf = vf_base + car.rotmat.z_axis * TOTAL_JUMP_ACC;
+            let xf = car.landing_location + xf_base + car.rotmat.z_axis * (time_remaining * PARITAL_JUMP_LOC + JUMP_LOC_P2);
 
             if let Some((jump_type, boost)) = basic_aerial_info.validate(xf, vf, AerialJumpType::Normal) {
                 found.push((jump_type, boost, true));
             }
         }
     }
 
     if target_angle_check(car.location) {
         let basic_aerial_info = BasicAerialInfo {
-            car_forward: car.forward,
+            car_forward: car.rotmat.x_axis,
             car_boost: f32::from(car.boost),
             boost_amount: mutators.boost_amount,
             boost_accel,
             target,
             time_remaining,
             // car,
         };
 
-        if !car.doublejumped
-            && (!is_on_ground || (car.airborne && (car.velocity.z + gravity.z * car.time_to_land) + mutators.boost_accel * car.time_to_land + JUMP_SPEED > 0.))
+        if car.car_state != State::DoubleJumped
+            && (!is_on_ground
+                || (car.car_state != State::Grounded && (car.velocity.z + gravity.z * car.time_to_land) + mutators.boost_accel * car.time_to_land + JUMP_SPEED > 0.))
         {
-            let vf = vf_base + car.up * JUMP_SPEED;
-            let xf = car.location + xf_base + car.up * (JUMP_SPEED * time_remaining);
+            let vf = vf_base + car.rotmat.z_axis * JUMP_SPEED;
+            let xf = car.location + xf_base + car.rotmat.z_axis * (JUMP_SPEED * time_remaining);
 
             if let Some((jump_type, boost)) = basic_aerial_info.validate(xf, vf, AerialJumpType::Secondary) {
                 found.push((jump_type, boost, false));
             }
         }
 
-        if !is_on_ground || car.up.z < 0. || (car.airborne && (car.velocity.z + gravity.z * car.time_to_land) + mutators.boost_accel * car.time_to_land > 0.) {
+        if !is_on_ground
+            || car.rotmat.z_axis.z < 0.
+            || (car.car_state != State::Grounded && (car.velocity.z + gravity.z * car.time_to_land) + mutators.boost_accel * car.time_to_land > 0.)
+        {
             if let Some((jump_type, boost)) = basic_aerial_info.validate(car.location + xf_base, vf_base, AerialJumpType::None) {
                 found.push((jump_type, boost, false));
             }
         }
     }
 
     if found.is_empty() {
```

### Comparing `VirxERLU_RLib-1.1.1/src/analyzer.rs` & `VirxERLU_RLib-1.1.2/src/analyzer.rs`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 use dubins_paths::{mod2pi, DubinsPath, NoPathError, PathType, PosRot, Result as DubinsResult};
 use glam::Vec3A;
 use rl_ball_sym::simulation::ball::Ball;
 
 use crate::{
     air::{aerial_shot_is_viable, AerialTargetInfo},
-    car::Car,
+    car::{Car, State},
     ground::{angle_2d, get_turn_exit_tanget, shortest_path_in_validate, GroundTargetInfo},
     pytypes::ShotType,
     utils::flatten,
     Mutators,
 };
 
 #[derive(Clone, Copy, Debug, PartialEq, Eq)]
@@ -68,15 +68,15 @@
             if self.may_shoot(Shot::Jump) {
                 return Ok(ShotType::Jump);
             }
         } else if target.z < self.car.max_double_jump_height && self.may_shoot(Shot::DoubleJump) {
             return Ok(ShotType::DoubleJump);
         }
 
-        if self.car.airborne || self.car.wait_to_jump_time + self.car.last_landing_time < time_remaining && self.may_shoot(Shot::Aerial) {
+        if self.car.car_state != State::Grounded || self.car.wait_to_jump_time + self.car.last_landing_time < time_remaining && self.may_shoot(Shot::Aerial) {
             return Ok(ShotType::Aerial);
         }
 
         Err(NoPathError)
     }
 
     fn get_jump_info(
@@ -89,17 +89,17 @@
         shot_type: ShotType,
     ) -> DubinsResult<(Option<f32>, f32)> {
         Ok(match shot_type {
             ShotType::Ground => {
                 let distance = 320.;
                 (
                     None,
-                    if (0. ..distance).contains(&self.car.forward.dot(ball_location))
-                        && self.car.right.dot(ball_location) < self.car.hitbox.width / 2.
-                        && angle_2d(self.car.forward, shot_vector) < 0.02
+                    if (0. ..distance).contains(&self.car.rotmat.x_axis.dot(ball_location))
+                        && self.car.rotmat.y_axis.dot(ball_location) < self.car.hitbox.width / 2.
+                        && angle_2d(self.car.rotmat.x_axis, shot_vector) < 0.02
                     {
                         0. // for pre-aligned ground shots
                     } else {
                         distance // for non-aligned ground shots
                     },
                 )
             }
@@ -158,15 +158,22 @@
         }
 
         let rho = self.get_max_turn_radius(slice_num);
         let is_forwards = self.should_travel_forwards(time_remaining, car_to_ball);
         let local_ball = self.car.localize_2d_location(ball.location);
         let target_is_forwards = local_ball.x >= 0.;
         let should_turn_left = local_ball.y < 0.;
-        let center_of_turn = car_location + flatten(if should_turn_left { -self.car.landing_right } else { self.car.landing_right } * rho);
+        let center_of_turn = car_location
+            + flatten(
+                if should_turn_left {
+                    -self.car.landing_rotmat.y_axis
+                } else {
+                    self.car.landing_rotmat.y_axis
+                } * rho,
+            );
 
         let (turn_target, turn_target_2) = get_turn_exit_tanget(self.car, flatten(ball.location), center_of_turn, rho, target_is_forwards, is_forwards);
 
         // check if the exit point is in the field
         if !self.car.field.is_point_in(turn_target) {
             return Err(NoPathError);
         }
@@ -179,17 +186,17 @@
         if turn_final_distance < offset_distance || turn_final_distance + turn_target.distance(car_location) > max_distance {
             return Err(NoPathError);
         }
 
         let shot_vector = (flatten(ball.location) - turn_target).normalize_or_zero();
         let shot_vector_angle = shot_vector.y.atan2(shot_vector.x);
         let forward_angle = if is_forwards {
-            self.car.landing_forward.y.atan2(self.car.landing_forward.x)
+            self.car.landing_rotmat.x_axis.y.atan2(self.car.landing_rotmat.x_axis.x)
         } else {
-            let forward = self.car.landing_forward * Vec3A::NEG_ONE;
+            let forward = self.car.landing_rotmat.x_axis * Vec3A::NEG_ONE;
             forward.y.atan2(forward.x)
         };
 
         let direction_turn_left = (is_forwards && should_turn_left) || (!is_forwards && !should_turn_left);
 
         // find the angle between the car location and each turn exit point relative to the exit turn point centers
         let turn_angle = mod2pi(if direction_turn_left {
@@ -220,15 +227,15 @@
             distances,
             shot_type,
             path,
             jump_time,
             is_forwards,
             shot_vector,
             turn_targets: Some((turn_target, turn_target_2)),
-            wait_for_land: self.car.airborne,
+            wait_for_land: self.car.car_state != State::Grounded,
         })
     }
 
     pub fn target(&self, ball: &Ball, shot_vector: Vec3A, mut time_remaining: f32, slice_num: usize, shot_type: ShotType) -> DubinsResult<GroundTargetInfo> {
         let offset_target = ball.location - (shot_vector * ball.radius());
         let car_front_length = (self.car.hitbox_offset.x + self.car.hitbox.length) / 2.;
 
@@ -282,15 +289,15 @@
             distances,
             shot_type,
             path,
             jump_time,
             is_forwards,
             shot_vector,
             turn_targets: None,
-            wait_for_land: self.car.airborne,
+            wait_for_land: self.car.car_state != State::Grounded,
         })
     }
 
     #[inline]
     pub fn aerial_shot(
         &self,
         mutators: Mutators,
```

### Comparing `VirxERLU_RLib-1.1.1/src/car.rs` & `VirxERLU_RLib-1.1.2/src/car.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-use dubins_paths::DubinsPath;
-use glam::Vec3A;
+use dubins_paths::{DubinsPath, PosRot};
+use glam::{Mat3A, Quat, Vec3A};
 
 use crate::{
     constants::*,
     pytypes::{GameCar, Hitbox},
     utils::{flatten, minimum_non_negative, vertex_quadratic_solve_for_x},
     BoostAmount, Mutators,
 };
 
-pub fn throttle_acceleration(forward_velocity: f32) -> f32 {
-    let x = forward_velocity.abs();
-
-    if x >= MAX_SPEED_NO_BOOST {
-        return 0.;
-    }
-
-    // use y = mx + b to find the throttle acceleration
-    if x < THROTTLE_ACCEL_DIVISION {
-        START_THROTTLE_ACCEL_M * x + START_THROTTLE_ACCEL_B
+#[must_use]
+pub fn throttle_acceleration(mut forward_velocity: f32) -> f32 {
+    forward_velocity = forward_velocity.abs();
+
+    if forward_velocity >= MAX_SPEED_NO_BOOST {
+        0.
+    } else if forward_velocity < THROTTLE_ACCEL_DIVISION {
+        START_THROTTLE_ACCEL_M * forward_velocity + START_THROTTLE_ACCEL_B
     } else {
-        END_THROTTLE_ACCEL_M * (x - THROTTLE_ACCEL_DIVISION) + END_THROTTLE_ACCEL_B
+        END_THROTTLE_ACCEL_M * forward_velocity - END_THROTTLE_ACCEL_M * THROTTLE_ACCEL_DIVISION + END_THROTTLE_ACCEL_B
     }
 }
 
-pub fn curvature(v: f32) -> f32 {
-    let v = v.abs();
+#[must_use]
+pub fn curvature(mut v: f32) -> f32 {
+    v = v.copysign(1.);
 
     if (0. ..500.).contains(&v) {
         0.0069 - 5.84e-6 * v
     } else if (500. ..1000.).contains(&v) {
         0.00561 - 3.26e-6 * v
     } else if (1000. ..1500.).contains(&v) {
         0.0043 - 1.95e-6 * v
@@ -39,14 +38,15 @@
     } else {
         println!("Invalid input velocity: {v}");
         -1.
     }
 }
 
 #[inline]
+#[must_use]
 pub fn turn_radius(v: f32) -> f32 {
     1. / curvature(v)
 }
 
 #[derive(Clone, Copy, Debug, Default)]
 pub struct FieldRect {
     goal_x: f32,
@@ -55,88 +55,125 @@
     field_x: f32,
 }
 
 impl FieldRect {
     const CHECK_DISTANCE: f32 = 400.;
 
     #[inline]
+    #[must_use]
     pub const fn new() -> Self {
         Self {
             goal_x: 0.,
             goal_y: 0.,
             field_y: 0.,
             field_x: 0.,
         }
     }
 
+    #[must_use]
     pub fn from(car_hitbox: &Hitbox) -> Self {
         let half_car_len = car_hitbox.length / 2.;
 
         Self {
             goal_x: 893. - car_hitbox.width,
             goal_y: 6000. - car_hitbox.length,
             field_y: 5120. - half_car_len,
             field_x: 4093. - half_car_len,
         }
     }
 
+    #[must_use]
     pub fn is_path_in(&self, path: &DubinsPath) -> bool {
         let length = path.length();
 
+        let types = path.type_.to_segment_types();
+
+        let qi = PosRot {
+            pos: Vec3A::ZERO,
+            rot: path.qi.rot,
+        };
+
+        let q1 = DubinsPath::segment(path.param[0], qi, types[0]);
+        let q2 = DubinsPath::segment(path.param[1], q1, types[1]);
+
         let mut dist = Self::CHECK_DISTANCE.min(length / 2.);
 
         while dist < length {
-            if !self.is_point_in(path.sample(dist).pos) {
+            let tprime = dist / path.rho;
+
+            let q = if tprime < path.param[0] {
+                DubinsPath::segment(tprime, qi, types[0])
+            } else if tprime < path.param[0] + path.param[1] {
+                DubinsPath::segment(tprime - path.param[0], q1, types[1])
+            } else {
+                DubinsPath::segment(tprime - path.param[0] - path.param[1], q2, types[2])
+            };
+
+            let sample = (q.pos * path.rho) + path.qi.pos;
+
+            if !self.is_point_in(sample) {
                 return false;
             }
 
             dist += Self::CHECK_DISTANCE;
         }
 
         true
     }
 
+    #[must_use]
     pub fn is_point_in(&self, p: Vec3A) -> bool {
         let p = [p.x.abs(), p.y.abs()];
 
         if p[0] > self.goal_x {
             p[0] < self.field_x && p[1] < self.field_y
         } else {
             p[1] < self.goal_y
         }
     }
 }
 
+#[derive(Clone, Copy, Debug, Default, PartialEq, Eq)]
+pub enum State {
+    Demolished,
+    #[default]
+    Grounded,
+    Jumped,
+    DoubleJumped,
+    Floating,
+}
+
 #[derive(Clone, Debug)]
 pub struct Car {
     pub location: Vec3A,
     pub velocity: Vec3A,
     pub local_velocity: Vec3A,
     pub angular_velocity: Vec3A,
-    pub forward: Vec3A,
-    pub right: Vec3A,
-    pub up: Vec3A,
+    // pub forward: Vec3A,
+    // pub right: Vec3A,
+    // pub up: Vec3A,
+    pub rotmat: Mat3A,
+    pub quat: Quat,
     pub hitbox: Hitbox,
     pub hitbox_offset: Vec3A,
     pub field: FieldRect,
     pub pitch: f32,
     pub yaw: f32,
     pub roll: f32,
     pub boost: u8,
-    pub demolished: bool,
-    pub airborne: bool,
-    pub jumped: bool,
-    pub doublejumped: bool,
+    pub car_state: State,
     pub time_to_land: f32,
     pub landing_location: Vec3A,
     pub landing_velocity: Vec3A,
     pub landing_yaw: f32,
-    pub landing_forward: Vec3A,
-    pub landing_right: Vec3A,
-    pub landing_up: Vec3A,
+    // pub landing_forward: Vec3A,
+    // pub landing_right: Vec3A,
+    // pub landing_up: Vec3A,
+    pub landing_rotmat: Mat3A,
+    pub landing_quat: Quat,
     last_landing_game_time: f32,
     pub last_landing_time: f32,
     pub max_speed: Vec<f32>,
     /// turn radius at calculated max speed
     pub ctrms: Vec<f32>,
     pub max_jump_time: f32,
     pub max_jump_height: f32,
@@ -144,41 +181,43 @@
     pub max_double_jump_height: f32,
     pub wait_to_jump_time: f32,
     pub init: bool,
 }
 
 impl Car {
     #[inline]
+    #[must_use]
     pub const fn new() -> Self {
         Self {
             location: Vec3A::ZERO,
             velocity: Vec3A::ZERO,
             local_velocity: Vec3A::ZERO,
             angular_velocity: Vec3A::ZERO,
-            forward: Vec3A::ZERO,
-            right: Vec3A::ZERO,
-            up: Vec3A::ZERO,
+            // forward: Vec3A::ZERO,
+            // right: Vec3A::ZERO,
+            // up: Vec3A::ZERO,
+            rotmat: Mat3A::IDENTITY,
+            quat: Quat::IDENTITY,
             hitbox: Hitbox::new(),
             hitbox_offset: Vec3A::ZERO,
             field: FieldRect::new(),
             pitch: 0.,
             yaw: 0.,
             roll: 0.,
             boost: 0,
-            demolished: false,
-            airborne: false,
-            jumped: false,
-            doublejumped: false,
+            car_state: State::Grounded,
             time_to_land: 0.,
             landing_location: Vec3A::ZERO,
             landing_velocity: Vec3A::ZERO,
             landing_yaw: 0.,
-            landing_forward: Vec3A::ZERO,
-            landing_right: Vec3A::ZERO,
-            landing_up: Vec3A::ZERO,
+            // landing_forward: Vec3A::ZERO,
+            // landing_right: Vec3A::ZERO,
+            // landing_up: Vec3A::ZERO,
+            landing_rotmat: Mat3A::IDENTITY,
+            landing_quat: Quat::IDENTITY,
             last_landing_game_time: 0.,
             last_landing_time: 0.,
             max_speed: Vec::new(),
             ctrms: Vec::new(),
             max_jump_time: 0.,
             max_jump_height: 0.,
             max_double_jump_time: 0.,
@@ -197,33 +236,39 @@
         self.yaw = py_car.physics.rotation.yaw;
         self.roll = py_car.physics.rotation.roll;
 
         self.hitbox = py_car.hitbox;
         self.hitbox_offset = py_car.hitbox_offset.into();
 
         self.boost = py_car.boost;
-        self.demolished = py_car.is_demolished;
-        self.jumped = py_car.jumped;
-        self.doublejumped = py_car.double_jumped;
-
-        let airborne = !py_car.has_wheel_contact;
 
-        if self.airborne && !airborne {
+        if self.car_state != State::Grounded && py_car.has_wheel_contact {
             self.last_landing_game_time = game_time;
         }
 
         self.last_landing_time = self.last_landing_game_time - game_time;
-        self.airborne = airborne;
+
+        if py_car.is_demolished {
+            self.car_state = State::Demolished;
+        } else if py_car.has_wheel_contact {
+            self.car_state = State::Grounded;
+        } else if py_car.double_jumped {
+            self.car_state = State::DoubleJumped;
+        } else if py_car.jumped {
+            self.car_state = State::Jumped;
+        } else {
+            self.car_state = State::Floating;
+        }
 
         self.init = false;
     }
 
     pub fn init(&mut self, gravity: f32, max_ball_slice: usize, mutators: Mutators) {
         if !self.init {
-            Self::calculate_orientation_matrix(&mut self.forward, &mut self.right, &mut self.up, self.pitch, self.yaw, self.roll);
+            Self::calculate_orientation_matrix(&mut self.quat, &mut self.rotmat, self.pitch, self.yaw, self.roll);
             self.calculate_field();
             self.calculate_landing_info(gravity);
             self.calculate_local_values();
             self.calculate_max_values(max_ball_slice, mutators);
             self.calculate_max_jump_height(gravity);
             self.calculate_max_double_jump_height(gravity);
 
@@ -294,27 +339,26 @@
     }
 
     fn calculate_landing_info(&mut self, gravity: f32) {
         self.time_to_land = 0.;
         self.landing_location = self.location;
         self.landing_velocity = self.velocity;
         self.landing_yaw = self.yaw;
-        self.landing_forward = self.forward;
-        self.landing_right = self.right;
-        self.landing_up = self.up;
+        self.landing_rotmat = Mat3A::from_cols(self.rotmat.x_axis, self.rotmat.y_axis, Vec3A::Z);
+        self.landing_quat = Quat::from_mat3a(&self.landing_rotmat.transpose());
 
-        self.wait_to_jump_time = if self.airborne {
+        self.wait_to_jump_time = if self.car_state != State::Grounded {
             ON_GROUND_WAIT_TIME
         } else if self.last_landing_time < -ON_GROUND_WAIT_TIME {
             0.
         } else {
             ON_GROUND_WAIT_TIME + self.last_landing_time
         };
 
-        if !self.airborne {
+        if self.car_state == State::Grounded {
             return;
         }
 
         // it's impossible to get true 0 gravity in RL
         // best you can get is a very small value
         // so we'll just ignore that edge case
 
@@ -368,38 +412,40 @@
             self.landing_location.z = if normal_gravity { 17. } else { 2300. };
         }
 
         if flatten(self.landing_velocity).length() != 0. {
             self.landing_yaw = self.landing_velocity.y.atan2(self.landing_velocity.x);
         }
 
-        Self::calculate_orientation_matrix(&mut self.landing_forward, &mut self.landing_right, &mut self.landing_up, 0., self.landing_yaw, 0.);
+        Self::calculate_orientation_matrix(&mut self.landing_quat, &mut self.landing_rotmat, 0., self.landing_yaw, 0.);
     }
 
-    fn calculate_orientation_matrix(forward: &mut Vec3A, right: &mut Vec3A, up: &mut Vec3A, pitch: f32, yaw: f32, roll: f32) {
+    fn calculate_orientation_matrix(quat: &mut Quat, rotmat: &mut Mat3A, pitch: f32, yaw: f32, roll: f32) {
         let (s_p, c_p) = pitch.sin_cos();
         let (s_y, c_y) = yaw.sin_cos();
         let (s_r, c_r) = roll.sin_cos();
 
-        forward.x = c_p * c_y;
-        forward.y = c_p * s_y;
-        forward.z = s_p;
-
-        right.x = c_y * s_p * s_r - c_r * s_y;
-        right.y = s_y * s_p * s_r + c_r * c_y;
-        right.z = -c_p * s_r;
-
-        up.x = -c_r * c_y * s_p - s_r * s_y;
-        up.y = -c_r * s_y * s_p + s_r * c_y;
-        up.z = c_p * c_r;
+        rotmat.x_axis.x = c_p * c_y;
+        rotmat.x_axis.y = c_p * s_y;
+        rotmat.x_axis.z = s_p;
+
+        rotmat.y_axis.x = c_y * s_p * s_r - c_r * s_y;
+        rotmat.y_axis.y = s_y * s_p * s_r + c_r * c_y;
+        rotmat.y_axis.z = -c_p * s_r;
+
+        rotmat.z_axis.x = -c_r * c_y * s_p - s_r * s_y;
+        rotmat.z_axis.y = -c_r * s_y * s_p + s_r * c_y;
+        rotmat.z_axis.z = c_p * c_r;
+
+        *quat = Quat::from_mat3a(&rotmat.transpose());
     }
 
     fn calculate_max_values(&mut self, max_ball_slice: usize, mutators: Mutators) {
         let mut b = f32::from(self.boost);
-        let mut v = self.landing_velocity.dot(self.forward);
+        let mut v = self.landing_velocity.dot(self.rotmat.x_axis);
         let mut fast_forward = false;
 
         self.max_speed = Vec::with_capacity(max_ball_slice);
         self.max_speed.push(v);
 
         self.ctrms = Vec::with_capacity(max_ball_slice);
         self.ctrms.push(turn_radius(v));
@@ -521,36 +567,40 @@
     }
 
     fn calculate_field(&mut self) {
         self.field = FieldRect::from(&self.hitbox);
     }
 
     #[inline]
+    #[must_use]
     pub fn localize_2d_location(&self, vec: Vec3A) -> Vec3A {
         self.localize_2d(vec - self.landing_location)
     }
 
     #[inline]
+    #[must_use]
     pub fn localize_2d(&self, vec: Vec3A) -> Vec3A {
-        Vec3A::new(vec.dot(self.landing_forward), vec.dot(self.landing_right), 0.)
+        self.landing_quat * vec
     }
 
     // pub fn localize_location(car: &Car, vec: Vec3A) -> Vec3A {
     //     localize(car, vec - car.location)
     // }
 
     #[inline]
+    #[must_use]
     pub fn localize(&self, vec: Vec3A) -> Vec3A {
-        Vec3A::new(vec.dot(self.forward), vec.dot(self.right), vec.dot(self.up))
+        self.quat * vec
     }
 
     // pub fn globalize(car: &Car, vec: Vec3A) -> Vec3A {
     //     car.forward * vec.x + car.right * vec.y + car.up * vec.z + car.location
     // }
 
+    #[must_use]
     pub fn jump_time_to_height(&self, gravity: f32, height_goal: f32) -> f32 {
         let g = gravity * SIMULATION_DT;
 
         let mut t = 0.;
         let mut v_z = self.landing_velocity.z;
         let mut l_z = self.landing_location.z;
 
@@ -571,14 +621,15 @@
             v_z += g;
             l_z += v_z * SIMULATION_DT;
         }
 
         t
     }
 
+    #[must_use]
     pub fn double_jump_time_to_height(&self, gravity: f32, height_goal: f32) -> f32 {
         let g = gravity * SIMULATION_DT;
 
         let mut t = 0.;
         let mut v_z = self.landing_velocity.z;
         let mut l_z = self.landing_location.z;
         let mut double_jumped = false;
@@ -607,15 +658,15 @@
         t
     }
 }
 
 #[cfg(test)]
 mod tests {
     use crate::{
-        car::{Car, Hitbox},
+        car::{Car, Hitbox, State},
         Mutators, Vec3A,
     };
 
     #[test]
     pub fn init_car() {
         let mut car = Car::new();
 
@@ -629,15 +680,12 @@
         car.hitbox = Hitbox {
             length: 118.,
             width: 84.2,
             height: 36.2,
         };
         car.hitbox_offset = Vec3A::new(13.9, 0., 20.8);
         car.boost = 48;
-        car.demolished = false;
-        car.airborne = false;
-        car.jumped = false;
-        car.doublejumped = false;
+        car.car_state = State::Grounded;
 
         car.init(-650., 720, Mutators::new());
     }
 }
```

### Comparing `VirxERLU_RLib-1.1.1/src/constants.rs` & `VirxERLU_RLib-1.1.2/src/constants.rs`

 * *Files identical despite different names*

### Comparing `VirxERLU_RLib-1.1.1/src/ground.rs` & `VirxERLU_RLib-1.1.2/src/ground.rs`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     let (d1s, d1c) = (d + th).sin_cos();
     let (d2s, d2c) = (d - th).sin_cos();
 
     (circle_center + radius * Vec3A::new(d1c, d1s, 0.), circle_center + radius * Vec3A::new(d2c, d2s, 0.))
 }
 
 /// Get the exit turn point on a circle where the car will face the target
+#[must_use]
 pub fn get_turn_exit_tanget(car: &Car, target: Vec3A, circle_center: Vec3A, rho: f32, mut target_is_forwards: bool, travel_forwards: bool) -> (Vec3A, Vec3A) {
     let (t1, t2) = get_turn_exit_tangets(target, circle_center, rho);
     let (mut t1_local, mut t2_local) = (car.localize_2d_location(t1), car.localize_2d_location(t2));
 
     if !travel_forwards {
         t1_local.x *= -1.;
         t2_local.x *= -1.;
@@ -50,14 +51,15 @@
         (t1, t2)
     } else {
         (t2, t1)
     }
 }
 
 #[inline]
+#[must_use]
 pub fn angle_2d(vec1: Vec3A, vec2: Vec3A) -> f32 {
     flatten(vec1).normalize_or_zero().dot(flatten(vec2).normalize_or_zero()).clamp(-1., 1.).acos()
 }
 
 pub fn shortest_path_in_validate(q0: PosRot, q1: PosRot, rho: f32, car_field: &FieldRect, max_distance: f32) -> DubinsResult<DubinsPath> {
     let mut best_cost = INFINITY;
     let mut best_path = None;
@@ -81,27 +83,34 @@
         }
     }
 
     best_path.ok_or(NoPathError)
 }
 
 #[derive(Clone, Copy, Debug)]
+pub enum CantReachError {
+    NoTime,
+    ForwardsReqTooFast,
+    BackwardsReqTooFast,
+}
+
+#[derive(Clone, Copy, Debug)]
 pub struct GroundTargetInfo {
     pub distances: [f32; 4],
     pub path: DubinsPath,
     pub shot_type: ShotType,
     pub jump_time: Option<f32>,
     pub is_forwards: bool,
     pub shot_vector: Vec3A,
     pub turn_targets: Option<(Vec3A, Vec3A)>,
     pub wait_for_land: bool,
 }
 
 impl GroundTargetInfo {
-    pub fn can_reach(&self, car: &Car, max_time: f32, mutators: Mutators) -> Result<f32, ()> {
+    pub fn can_reach(&self, car: &Car, max_time: f32, mutators: Mutators) -> Result<f32, CantReachError> {
         let is_curved = PathType::CCC.contains(&self.path.type_);
 
         let total_d = self.distances.iter().sum::<f32>();
 
         let middle_range = {
             let start = self.distances[0];
             let end = start + self.distances[1];
@@ -113,21 +122,25 @@
 
         let mut d = total_d;
         let mut t_r = max_time;
         let b_s = f32::from(car.boost.min(12));
         let mut b = f32::from(car.boost) - b_s;
         let mut v = flatten(car.landing_velocity).length() * direction;
 
+        let boost_accel = if mutators.boost_amount == BoostAmount::NoBoost { 0. } else { mutators.boost_accel };
+
+        let boost_consumption_dt = if mutators.boost_amount == BoostAmount::Unlimited { 0. } else { BOOST_CONSUMPTION_DT };
+
         loop {
             if self.distances[3] < f32::EPSILON && d < 1. {
                 return Ok(t_r.max(0.));
             }
 
             if t_r <= 0. {
-                return Err(());
+                return Err(CantReachError::NoTime);
             }
 
             let r = d * direction / t_r;
             let t = r - v;
 
             let distance_traveled = total_d - d;
             let is_middle_straight = !is_curved && middle_range.contains(&distance_traveled);
@@ -146,55 +159,48 @@
                         continue;
                     }
                 }
             }
 
             if self.is_forwards {
                 let quick_max_speed = if b >= 1. {
-                    MAX_SPEED.min(MAX_SPEED_NO_BOOST.max(v) + BOOST_ACCEL * t_r.min(b / BOOST_CONSUMPTION))
+                    MAX_SPEED.min(MAX_SPEED_NO_BOOST.max(v) + boost_accel * t_r.min(b / BOOST_CONSUMPTION))
                 } else {
                     MAX_SPEED_NO_BOOST.max(v)
                 };
 
                 if r > quick_max_speed {
-                    return Err(());
+                    return Err(CantReachError::ForwardsReqTooFast);
                 }
             } else if MIN_SPEED > r {
-                return Err(());
+                return Err(CantReachError::BackwardsReqTooFast);
             }
 
             let throttle_accel = throttle_acceleration(v);
-            let (throttle, boost) = {
-                let (mut throttle, mut boost) = get_throttle_and_boost(throttle_accel, b, if v < 0. { -t } else { t });
+            let (mut throttle, mut boost) = get_throttle_and_boost(throttle_accel, b, t.copysign(v), boost_accel);
 
-                if t <= 0. {
-                    boost = false;
-                }
+            if t <= 0. {
+                boost = false;
+            }
 
-                if v < 0. {
-                    throttle *= -1.;
-                }
+            throttle *= 1f32.copysign(v);
 
-                (throttle, boost)
-            };
             let mut accel = 0.;
 
-            if throttle == 0. {
-                accel += COAST_ACC * SIMULATION_DT * -v.signum();
-            } else if throttle.signum() == v.signum() {
-                accel += throttle_accel * SIMULATION_DT * throttle;
+            accel += if throttle == 0. {
+                COAST_ACC * SIMULATION_DT * 1f32.copysign(-v)
+            } else if throttle * v >= 0. {
+                throttle_accel * SIMULATION_DT * throttle
             } else {
-                accel += BRAKE_ACC_DT.copysign(throttle);
-            }
+                BRAKE_ACC_DT.copysign(throttle)
+            };
 
-            if mutators.boost_amount != BoostAmount::NoBoost && boost {
-                accel += mutators.boost_accel * SIMULATION_DT;
-                if mutators.boost_amount != BoostAmount::Unlimited {
-                    b -= BOOST_CONSUMPTION_DT;
-                }
+            if boost {
+                accel += boost_accel * SIMULATION_DT;
+                b -= boost_consumption_dt;
             }
 
             if !(is_middle_straight || d < self.distances[3]) {
                 accel -= self.path.rho / E * SIMULATION_DT;
                 accel = accel.min(2295. - v);
             }
 
@@ -205,29 +211,32 @@
             d -= d_delta;
         }
 
         Ok(t_r)
     }
 
     #[inline]
+    #[must_use]
     pub const fn get_basic_shot_info(&self, time: f32) -> BasicShotInfo {
         BasicShotInfo::found(time, self.shot_type, self.shot_vector, self.is_forwards, self.wait_for_land)
     }
 }
 
-fn get_throttle_and_boost(throttle_accel: f32, b: f32, t: f32) -> (f32, bool) {
+fn get_throttle_and_boost(throttle_accel: f32, b: f32, t: f32, boost_accel: f32) -> (f32, bool) {
     let acceleration = t / REACTION_TIME;
-    let throttle_boost_transition = throttle_accel + 0.5 * BOOST_ACCEL;
 
     if acceleration <= BRAKE_COAST_TRANSITION {
         (-1., false)
     } else if BRAKE_COAST_TRANSITION < acceleration && acceleration < COASTING_THROTTLE_TRANSITION {
         (0., false)
-    } else if (COASTING_THROTTLE_TRANSITION..throttle_boost_transition).contains(&acceleration) {
-        let throttle = if throttle_accel == 0. { 1. } else { (acceleration / throttle_accel).clamp(0.02, 1.) };
-        (throttle, false)
-    } else if throttle_boost_transition < acceleration {
-        (1., b >= MIN_BOOST_CONSUMPTION && t > 0.)
     } else {
-        (0., false)
+        let throttle_boost_transition = throttle_accel + 0.5 * boost_accel;
+        if (COASTING_THROTTLE_TRANSITION..throttle_boost_transition).contains(&acceleration) {
+            let throttle = if throttle_accel == 0. { 1. } else { (acceleration / throttle_accel).clamp(0.02, 1.) };
+            (throttle, false)
+        } else if throttle_boost_transition < acceleration {
+            (1., b >= MIN_BOOST_CONSUMPTION && t > 0.)
+        } else {
+            (0., false)
+        }
     }
 }
```

### Comparing `VirxERLU_RLib-1.1.1/src/lib.rs` & `VirxERLU_RLib-1.1.2/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #![forbid(unsafe_code)]
 
-mod air;
-mod analyzer;
-mod car;
-mod constants;
-mod ground;
-mod pytypes;
-mod shot;
-mod utils;
+pub mod air;
+pub mod analyzer;
+pub mod car;
+pub mod constants;
+pub mod ground;
+pub mod pytypes;
+pub mod shot;
+pub mod utils;
 
 use std::sync::RwLock;
 
 use combo_vec::{rearr, ReArr};
 use glam::Vec3A;
 use pyo3::prelude::*;
 use rl_ball_sym::simulation::{
     ball::{Ball, Predictions},
     game::Game,
 };
 
 use analyzer::*;
-use car::{turn_radius, Car};
+use car::{turn_radius, Car, State};
 use constants::*;
 use pytypes::*;
 use shot::{AirBasedShot, GroundBasedShot, Options, Shot, Target};
 use utils::*;
 
 static CARS: RwLock<ReArr<Car, 8>> = RwLock::new(rearr![]);
 static BALL_STRUCT: RwLock<Predictions> = RwLock::new(Predictions::new());
@@ -54,39 +54,39 @@
     tick, get_slice, get_slice_index, get_num_ball_slices, set_mutator_settings,
     new_target, new_any_target, confirm_target, remove_target, print_targets, get_targets_length,
     get_shot_with_target, get_data_for_shot_with_target],
     classes: [TargetOptions, ShotType, BallSlice, BasicShotInfo, AdvancedShotInfo]
 );
 
 #[pyfunction]
-fn load_standard() {
+pub fn load_standard() {
     let (game, ball) = rl_ball_sym::compressed::load_standard();
 
     *GAME.write().unwrap() = Some(game);
     *BALL.write().unwrap() = ball;
 }
 
 #[pyfunction]
-fn load_dropshot() {
+pub fn load_dropshot() {
     let (game, ball) = rl_ball_sym::compressed::load_dropshot();
 
     *GAME.write().unwrap() = Some(game);
     *BALL.write().unwrap() = ball;
 }
 
 #[pyfunction]
-fn load_hoops() {
+pub fn load_hoops() {
     let (game, ball) = rl_ball_sym::compressed::load_hoops();
 
     *GAME.write().unwrap() = Some(game);
     *BALL.write().unwrap() = ball;
 }
 
 #[pyfunction]
-fn load_standard_throwback() {
+pub fn load_standard_throwback() {
     let (game, ball) = rl_ball_sym::compressed::load_standard_throwback();
 
     *GAME.write().unwrap() = Some(game);
     *BALL.write().unwrap() = ball;
 }
 
 #[derive(Clone, Copy, Debug, PartialEq, Eq)]
@@ -142,22 +142,22 @@
                 _ => BOOST_ACCEL,
             },
         })
     }
 }
 
 #[pyfunction]
-fn set_mutator_settings(mutators: &PyAny) -> PyResult<()> {
+pub fn set_mutator_settings(mutators: &PyAny) -> PyResult<()> {
     *MUTATORS.write().unwrap() = Mutators::try_from(mutators)?;
 
     Ok(())
 }
 
 #[pyfunction]
-fn tick(packet: GamePacket, prediction_time: Option<f32>) -> PyResult<()> {
+pub fn tick(packet: GamePacket, prediction_time: Option<f32>) -> PyResult<()> {
     TARGETS.write().unwrap().iter_mut().for_each(|target| {
         if matches!(target, Some(t) if !t.is_confirmed()) {
             *target = None;
         }
     });
 
     let mut game_guard = GAME.write().unwrap();
@@ -201,32 +201,32 @@
         car.update(pycar, packet.game_info.seconds_elapsed);
     }
 
     Ok(())
 }
 
 #[pyfunction]
-fn get_slice(slice_time: f32) -> BallSlice {
+pub fn get_slice(slice_time: f32) -> BallSlice {
     let slice_num = ((slice_time - *GAME_TIME.read().unwrap()) * TPS).round() as usize;
     get_slice_index(slice_num)
 }
 
 #[pyfunction]
-fn get_slice_index(slice_num: usize) -> BallSlice {
+pub fn get_slice_index(slice_num: usize) -> BallSlice {
     let ball_struct = BALL_STRUCT.read().unwrap();
     ball_struct[slice_num.clamp(0, ball_struct.len() - 1)].into()
 }
 
 #[pyfunction]
-fn get_num_ball_slices() -> usize {
+pub fn get_num_ball_slices() -> usize {
     BALL_STRUCT.read().unwrap().len()
 }
 
 #[pyfunction]
-fn new_target(left_target: [f32; 3], right_target: [f32; 3], car_index: usize, options: Option<TargetOptions>) -> PyResult<usize> {
+pub fn new_target(left_target: [f32; 3], right_target: [f32; 3], car_index: usize, options: Option<TargetOptions>) -> PyResult<usize> {
     let num_slices = BALL_STRUCT.read().unwrap().len();
 
     if num_slices == 0 {
         return Err(PyErr::new::<NoSlicesPyErr, _>(NO_SLICES_ERR));
     }
 
     let options = Options::new(options, num_slices);
@@ -249,15 +249,15 @@
         targets.len() - 1
     };
 
     Ok(target_index)
 }
 
 #[pyfunction]
-fn new_any_target(car_index: usize, options: Option<TargetOptions>) -> PyResult<usize> {
+pub fn new_any_target(car_index: usize, options: Option<TargetOptions>) -> PyResult<usize> {
     let num_slices = BALL_STRUCT.read().unwrap().len();
 
     if num_slices == 0 {
         return Err(PyErr::new::<NoSlicesPyErr, _>(NO_SLICES_ERR));
     }
 
     let options = Options::new(options, num_slices);
@@ -280,15 +280,15 @@
         targets.len() - 1
     };
 
     Ok(target_index)
 }
 
 #[pyfunction]
-fn confirm_target(target_index: usize) -> PyResult<()> {
+pub fn confirm_target(target_index: usize) -> PyResult<()> {
     let mut targets = TARGETS.write().unwrap();
     let target = targets
         .get_mut(target_index)
         .ok_or_else(|| PyErr::new::<NoTargetPyErr, _>(NO_TARGET_ERR))?
         .as_mut()
         .ok_or_else(|| PyErr::new::<NoTargetPyErr, _>(NO_TARGET_ERR))?;
 
@@ -297,25 +297,25 @@
     }
 
     target.confirm();
     Ok(())
 }
 
 #[pyfunction]
-fn remove_target(target_index: usize) {
+pub fn remove_target(target_index: usize) {
     let mut targets = TARGETS.write().unwrap();
     if targets.get(target_index).is_none() {
         return;
     }
 
     targets[target_index] = None;
 }
 
 #[pyfunction]
-fn print_targets() {
+pub fn print_targets() {
     let targets = TARGETS.read().unwrap();
     let mut out = Vec::with_capacity(targets.len());
 
     for target in targets.iter() {
         out.push(match target {
             Some(t) => match &t.shot {
                 Some(s) => s.time().to_string(),
@@ -325,15 +325,15 @@
         });
     }
 
     println!("[{}]", out.join(", "));
 }
 
 #[pyfunction]
-fn get_targets_length() -> usize {
+pub fn get_targets_length() -> usize {
     TARGETS.read().unwrap().len()
 }
 
 fn analyze_shot(analyzer: &Analyzer, balls: &Predictions, target: &Target, mutators: Mutators, temporary: bool, game_time: f32) -> Option<(Shot, BasicShotInfo)> {
     let mut shot = None;
 
     for (i, ball) in balls[target.options.min_slice..target.options.max_slice].iter().enumerate() {
@@ -344,15 +344,15 @@
         let max_time_remaining = ball.time - game_time;
 
         let Ok(shot_type) = analyzer.get_shot_type(ball.location, max_time_remaining) else {
             continue;
         };
 
         if let Some(target_location) = &target.location {
-            let post_info = PostCorrection::from(ball.location, ball.collision_radius(), target_location.left, target_location.right);
+            let post_info = PostCorrection::new(ball.location, ball.collision_radius(), target_location.left, target_location.right);
 
             if !post_info.fits {
                 continue;
             }
 
             let shot_vector = post_info.get_shot_vector_target(analyzer.car.landing_location, ball.location);
 
@@ -439,15 +439,15 @@
         }
     }
 
     shot
 }
 
 #[pyfunction]
-fn get_shot_with_target(
+pub fn get_shot_with_target(
     target_index: usize,
     temporary: Option<bool>,
     may_ground_shot: Option<bool>,
     may_jump_shot: Option<bool>,
     may_double_jump_shot: Option<bool>,
     may_aerial_shot: Option<bool>,
     only: Option<bool>,
@@ -479,15 +479,15 @@
             .ok_or_else(|| PyErr::new::<NoTargetPyErr, _>(NO_TARGET_ERR))?
             .as_ref()
             .ok_or_else(|| PyErr::new::<NoTargetPyErr, _>(NO_TARGET_ERR))?;
 
         let cars = CARS.read().unwrap();
         let car = cars.get(target.car_index).ok_or_else(|| PyErr::new::<NoCarPyErr, _>(NO_CAR_ERR))?;
 
-        if car.demolished || balls.is_empty() || car.time_to_land >= balls.last().map(|slice| slice.time).unwrap_or_default() {
+        if car.car_state == State::Demolished || balls.is_empty() || car.time_to_land >= balls.last().map(|slice| slice.time).unwrap_or_default() {
             return Ok(BasicShotInfo::not_found());
         }
 
         let (max_speed, max_turn_radius) = if target.options.use_absolute_max_values {
             (Some(MAX_SPEED), Some(turn_radius(MAX_SPEED)))
         } else {
             (None, None)
@@ -520,15 +520,15 @@
             .shot = Some(found_shot);
     }
 
     Ok(basic_shot_info)
 }
 
 #[pyfunction]
-fn get_data_for_shot_with_target(target_index: usize) -> PyResult<AdvancedShotInfo> {
+pub fn get_data_for_shot_with_target(target_index: usize) -> PyResult<AdvancedShotInfo> {
     let targets_gaurd = TARGETS.read().unwrap();
     let target = targets_gaurd
         .get(target_index)
         .ok_or_else(|| PyErr::new::<NoTargetPyErr, _>(NO_TARGET_ERR))?
         .as_ref()
         .ok_or_else(|| PyErr::new::<NoTargetPyErr, _>(NO_TARGET_ERR))?;
     let shot = target.shot.as_ref().ok_or_else(|| PyErr::new::<NoShotPyErr, _>(NO_SHOT_ERR))?;
```

### Comparing `VirxERLU_RLib-1.1.1/src/pytypes.rs` & `VirxERLU_RLib-1.1.2/src/pytypes.rs`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     pub length: f32,
     pub width: f32,
     pub height: f32,
 }
 
 impl Hitbox {
     #[inline]
+    #[must_use]
     pub const fn new() -> Self {
         Self {
             length: 0.,
             width: 0.,
             height: 0.,
         }
     }
@@ -72,23 +73,24 @@
     pub diameter: f32,
     pub height: f32,
 }
 
 #[derive(Clone, Copy, Debug, Default, FromPyObject)]
 pub struct GameCollisionShape {
     #[pyo3(attribute("type"))]
-    shape_type: usize,
+    pub shape_type: usize,
     #[pyo3(attribute("box"))]
-    box_: GameBox,
-    sphere: GameSphere,
-    cylinder: GameCylinder,
+    pub box_: GameBox,
+    pub sphere: GameSphere,
+    pub cylinder: GameCylinder,
 }
 
 impl GameCollisionShape {
     #[inline]
+    #[must_use]
     pub fn get_radius(&self) -> f32 {
         match self.shape_type {
             0 => (self.box_.length + self.box_.width + self.box_.height) / 6.,
             1 => self.sphere.diameter / 2.,
             2 => self.cylinder.diameter / 2.,
             _ => panic!("Invalid shape type: #{}", self.shape_type),
         }
@@ -143,14 +145,15 @@
     Jump,
     DoubleJump,
     Aerial,
 }
 
 impl ShotType {
     #[inline]
+    #[must_use]
     pub const fn to_str(self) -> &'static str {
         match self {
             ShotType::Ground => "Ground",
             ShotType::Jump => "Jump",
             ShotType::DoubleJump => "DoubleJump",
             ShotType::Aerial => "Aerial",
         }
@@ -231,26 +234,28 @@
     fn default() -> Self {
         Self::not_found()
     }
 }
 
 impl BasicShotInfo {
     #[inline]
+    #[must_use]
     pub const fn not_found() -> Self {
         BasicShotInfo {
             found: false,
             time: -1.,
             shot_type: None,
             shot_vector: (0., 0., 0.),
             is_forwards: true,
             wait_for_land: true,
         }
     }
 
     #[inline]
+    #[must_use]
     pub const fn found(time: f32, shot_type: ShotType, shot_vector: Vec3A, is_forwards: bool, wait_for_land: bool) -> Self {
         BasicShotInfo {
             found: true,
             time,
             shot_type: Some(shot_type),
             shot_vector: get_tuple_from_vec3(shot_vector),
             is_forwards,
@@ -314,19 +319,21 @@
     current_path_point: PyVec3A,
     turn_targets: Option<(PyVec3A, PyVec3A)>,
     num_jumps: Option<u8>,
 }
 
 impl AdvancedShotInfo {
     #[inline]
+    #[must_use]
     pub const fn get_distance_remaining(&self) -> f32 {
         self.distance_remaining
     }
 
     #[inline]
+    #[must_use]
     pub const fn get_final_target(&self) -> PyVec3A {
         self.final_target
     }
 }
 
 #[pymethods]
 impl AdvancedShotInfo {
@@ -383,14 +390,15 @@
                 None
             },
             num_jumps: None,
         })
     }
 
     #[inline]
+    #[must_use]
     pub fn get_from_air(car: &Car, shot: &AirBasedShot) -> Self {
         Self {
             final_target: get_tuple_from_vec3(shot.final_target),
             distance_remaining: car.location.distance(shot.final_target),
             path_samples: Vec::new(),
             required_jump_time: None,
             current_path_point: get_tuple_from_vec3(car.location),
```

### Comparing `VirxERLU_RLib-1.1.1/src/shot.rs` & `VirxERLU_RLib-1.1.2/src/shot.rs`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 use glam::Vec3A;
 use rl_ball_sym::simulation::ball::Ball;
 
 use crate::{
     air::{AerialJumpType, AerialTargetInfo},
     ground::GroundTargetInfo,
     pytypes::{ShotType, TargetOptions},
-    utils::{get_samples_from_line, get_samples_from_path},
+    utils::get_samples_from_line,
 };
 
 #[inline]
 const fn posrot_to_xy_tuple(posrot: &PosRot) -> (f32, f32) {
     let [x, y, _] = posrot.pos.to_array();
     (x, y)
 }
@@ -19,22 +19,24 @@
 pub enum Shot {
     GroundBased(Box<GroundBasedShot>),
     AirBased(AirBasedShot),
 }
 
 impl Shot {
     #[inline]
+    #[must_use]
     pub const fn time(&self) -> f32 {
         match self {
             Shot::GroundBased(shot) => shot.time,
             Shot::AirBased(shot) => shot.time,
         }
     }
 
     #[inline]
+    #[must_use]
     pub const fn ball_location(&self) -> Vec3A {
         match self {
             Shot::GroundBased(shot) => shot.ball_location,
             Shot::AirBased(shot) => shot.ball_location,
         }
     }
 }
@@ -59,14 +61,15 @@
     pub final_target: Vec3A,
     pub jump_type: AerialJumpType,
     pub ball_location: Vec3A,
 }
 
 impl AirBasedShot {
     #[inline]
+    #[must_use]
     pub const fn new(ball: &Ball, target_info: &AerialTargetInfo) -> Self {
         Self {
             time: ball.time,
             final_target: target_info.final_target,
             jump_type: target_info.jump_type,
             ball_location: ball.location,
         }
@@ -102,17 +105,17 @@
                 target.path.segment_length(0),
                 target.path.segment_length(0) + target.path.segment_length(1),
                 target.path.length(),
             ];
 
             // the samples for each subpath
             let raw_samples = [
-                get_samples_from_path(&target.path, 0., segment_distances[0], Self::STEP_DISTANCE),
-                get_samples_from_path(&target.path, segment_distances[0], segment_distances[1], Self::STEP_DISTANCE),
-                get_samples_from_path(&target.path, segment_distances[1], segment_distances[2], Self::STEP_DISTANCE),
+                target.path.sample_many_range(Self::STEP_DISTANCE, 0f32..segment_distances[0]),
+                target.path.sample_many_range(Self::STEP_DISTANCE, segment_distances[0]..segment_distances[1]),
+                target.path.sample_many_range(Self::STEP_DISTANCE, segment_distances[1]..segment_distances[2]),
                 get_samples_from_line(path_endpoint, direction, target.distances[3], Self::STEP_DISTANCE),
             ];
 
             (
                 raw_samples[0]
                     .iter()
                     .map(posrot_to_xy_tuple)
@@ -166,14 +169,15 @@
                 start_index = mid_index + 1;
             }
         }
 
         ((start_index + end_index) / 2, min_distance)
     }
 
+    #[must_use]
     pub fn find_min_distance_index(&self, target: Vec3A) -> (usize, usize) {
         let mut min_distance = f32::MAX;
         let mut min_distance_index = 0;
         let mut min_distance_index_in_section = 0;
 
         for segment in 0..self.samples.len() {
             let (index, distance) = self.find_min_distance_in_segment_index(segment, target);
@@ -184,14 +188,15 @@
                 min_distance_index_in_section = index;
             }
         }
 
         (min_distance_index, min_distance_index_in_section)
     }
 
+    #[must_use]
     pub fn get_distance_along_shot_and_index(&self, segment: usize, index: usize) -> (f32, usize) {
         let pre_distance = match segment {
             0 => 0.,
             1 => self.distances[0],
             2 => self.distances[0] + self.distances[1],
             3 => self.distances[0] + self.distances[1] + self.distances[2],
             _ => unreachable!(),
@@ -241,14 +246,15 @@
 pub struct TargetLocation {
     pub left: Vec3A,
     pub right: Vec3A,
 }
 
 impl TargetLocation {
     #[inline]
+    #[must_use]
     pub const fn new(left: Vec3A, right: Vec3A) -> Self {
         Self { left, right }
     }
 }
 
 #[derive(Clone, Debug, Default)]
 pub struct Target {
@@ -257,25 +263,27 @@
     pub options: Options,
     pub shot: Option<Shot>,
     confirmed: bool,
 }
 
 impl Target {
     #[inline]
+    #[must_use]
     pub const fn new(target_left: Vec3A, target_right: Vec3A, car_index: usize, options: Options) -> Self {
         Self {
             car_index,
             location: Some(TargetLocation::new(target_left, target_right)),
             options,
             shot: None,
             confirmed: false,
         }
     }
 
     #[inline]
+    #[must_use]
     pub const fn new_any(car_index: usize, options: Options) -> Self {
         Self {
             car_index,
             location: None,
             options,
             shot: None,
             confirmed: false,
@@ -284,11 +292,12 @@
 
     #[inline]
     pub fn confirm(&mut self) {
         self.confirmed = true;
     }
 
     #[inline]
+    #[must_use]
     pub const fn is_confirmed(&self) -> bool {
         self.confirmed
     }
 }
```

### Comparing `VirxERLU_RLib-1.1.1/src/utils.rs` & `VirxERLU_RLib-1.1.2/src/utils.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,31 @@
-use dubins_paths::{DubinsPath, PosRot};
+use dubins_paths::PosRot;
 use glam::Vec3A;
 use std::ops::{Add, Mul, Sub};
 
-/// Get a vec of samples from a path
-/// Starts at the given distance
-/// Ends at the given distance
-/// Step size is given
-pub fn get_samples_from_path(path: &DubinsPath, start_distance: f32, end_distance: f32, step_distance: f32) -> Vec<PosRot> {
-    let num_steps = ((end_distance - start_distance) / step_distance).ceil() as usize;
-    let mut samples = Vec::with_capacity(num_steps);
-    let mut distance = start_distance;
-
-    while distance < end_distance {
-        samples.push(path.sample(distance));
-        distance += step_distance;
-    }
-
-    samples
-}
-
 /// Get a vec of samples
 /// Starts at the given point
 /// Ends after the given distance
 /// Goes in the direction of the given vector
+#[must_use]
 pub fn get_samples_from_line(start: PosRot, direction: Vec3A, distance: f32, step_distance: f32) -> Vec<PosRot> {
     let mut samples = Vec::with_capacity((distance / step_distance).ceil() as usize);
     let mut current_distance = 0.;
 
     while current_distance < distance {
         let vec = start.pos + direction * current_distance;
         samples.push(PosRot::new(vec, start.rot));
         current_distance += step_distance;
     }
 
     samples
 }
 
 #[inline]
+#[must_use]
 pub const fn get_tuple_from_vec3(vec: Vec3A) -> (f32, f32, f32) {
     let [x, y, z] = vec.to_array();
     (x, y, z)
 }
 
 #[inline]
 pub fn lerp<T: Copy + Add<Output = T> + Sub<Output = T> + Mul<f32, Output = T>>(a: T, b: T, t: f32) -> T {
@@ -76,14 +61,15 @@
         ClampDirection::Right
     } else {
         ClampDirection::Left
     }
 }
 
 #[inline]
+#[must_use]
 pub const fn flatten(vec: Vec3A) -> Vec3A {
     let [x, y, _] = vec.to_array();
     Vec3A::new(x, y, 0.)
 }
 
 // fn clockwise90_2d(vec: Vec3A) -> Vec3A {
 //     Vec3A::new(vec.y, -vec.x, 0.)
@@ -97,73 +83,68 @@
 pub struct PostCorrection {
     pub target_left: Vec3A,
     pub target_right: Vec3A,
     pub fits: bool,
 }
 
 impl PostCorrection {
-    pub fn from(ball_location: Vec3A, ball_radius: f32, target_left: Vec3A, target_right: Vec3A) -> Self {
+    #[must_use]
+    pub fn new(ball_location: Vec3A, ball_radius: f32, target_left: Vec3A, target_right: Vec3A) -> Self {
         let goal_line_perp = (target_right - target_left).cross(Vec3A::Z);
 
-        let left_adjusted = target_left + (target_left - ball_location).normalize_or_zero().cross(-Vec3A::Z) * ball_radius;
-        let right_adjusted = target_right + (target_right - ball_location).normalize_or_zero().cross(Vec3A::Z) * ball_radius;
+        let left_adjusted = (target_left - ball_location).normalize().cross(-Vec3A::Z) * ball_radius;
+        let right_adjusted = (target_right - ball_location).normalize().cross(Vec3A::Z) * ball_radius;
+
+        let left_corrected = target_left + if left_adjusted.dot(goal_line_perp) > 0. { Vec3A::ZERO } else { left_adjusted };
 
-        let left_corrected = if (left_adjusted - target_left).dot(goal_line_perp) > 0. {
-            target_left
-        } else {
-            left_adjusted
-        };
-
-        let right_corrected = if (right_adjusted - target_right).dot(goal_line_perp) > 0. {
-            target_right
-        } else {
-            right_adjusted
-        };
+        let right_corrected = target_right + if right_adjusted.dot(goal_line_perp) > 0. { Vec3A::ZERO } else { right_adjusted };
 
         let left_to_right = right_corrected - left_corrected;
-        let new_goal_line = left_to_right.normalize_or_zero();
+        let new_goal_line = left_to_right.normalize();
         let new_goal_width = left_to_right.length();
 
         let new_goal_perp = new_goal_line.cross(Vec3A::Z);
         let goal_center = left_corrected + new_goal_line * new_goal_width * 0.5;
-        let ball_to_goal = (goal_center - ball_location).normalize_or_zero();
+        let ball_to_goal = (goal_center - ball_location).normalize();
 
         Self {
             target_left: left_corrected,
             target_right: right_corrected,
             fits: new_goal_width * new_goal_perp.dot(ball_to_goal).abs() > ball_radius * 2.,
         }
     }
 
+    #[must_use]
     pub fn get_shot_vector_target(&self, car_location: Vec3A, ball_location: Vec3A) -> Vec3A {
-        let left_vector = (self.target_left - ball_location).normalize_or_zero();
+        let left_vector = (self.target_left - ball_location).normalize();
         let left_vector_flat = flatten(left_vector);
-        let right_vector = (self.target_right - ball_location).normalize_or_zero();
+        let right_vector = (self.target_right - ball_location).normalize();
         let right_vector_flat = flatten(right_vector);
-        let car_to_ball_flat = flatten(ball_location - car_location).normalize_or_zero();
+        let car_to_ball_flat = flatten(ball_location - car_location).normalize();
 
         // All of this is so that the returned vector will always point towards the target z
         match clamp_index(car_to_ball_flat, left_vector_flat, right_vector_flat) {
             ClampDirection::Middle => {
                 // angle_between between uses acos, will always be between 0 and pi
                 let car_to_left_angle = left_vector_flat.angle_between(car_to_ball_flat);
                 let left_to_right_angle = left_vector_flat.angle_between(right_vector);
 
                 // convert angles to a value between 0 and 1
                 let t = car_to_left_angle / left_to_right_angle;
 
-                (lerp(self.target_left, self.target_right, t) - ball_location).normalize_or_zero()
+                (lerp(self.target_left, self.target_right, t) - ball_location).normalize()
             }
             ClampDirection::Left => left_vector,
             ClampDirection::Right => right_vector,
         }
     }
 }
 
 #[inline]
+#[must_use]
 pub fn minimum_non_negative(x1: f32, x2: f32) -> f32 {
     // get the smallest, non-negative value
     if x1 < 0. {
         x2
     } else if x2 < 0. {
         x1
     } else {
@@ -173,14 +154,15 @@
 
 // solve for x
 // y = a(x - h)^2 + k
 // y - k = a(x - h)^2
 // (y - k) / a = (x - h)^2
 // sqrt((y - k) / a) = x - h
 // sqrt((y - k) / a) + h = x
+#[must_use]
 pub fn vertex_quadratic_solve_for_x(a: f32, h: f32, k: f32, y: f32) -> (f32, f32) {
     if a == 0. {
         return (0., 0.);
     }
 
     let v_sqrt = ((y - k) / a).sqrt();
     (h + v_sqrt, h - v_sqrt)
```

### Comparing `VirxERLU_RLib-1.1.1/virx_erlu_rlib.pyi` & `VirxERLU_RLib-1.1.2/virx_erlu_rlib.pyi`

 * *Files identical despite different names*

### Comparing `VirxERLU_RLib-1.1.1/Cargo.lock` & `VirxERLU_RLib-1.1.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "dubins_paths"
-version = "1.6.0"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e24be98085e8b9dd5282d1b2d79ba5a41a69de8f19dcadca10ef7e81e584a84f"
+checksum = "38187dbbf076e5f2b85b5dd3e5fb37aa7ed99986e2b852bc08ea99e84c9d5ca8"
 dependencies = [
  "glam",
 ]
 
 [[package]]
 name = "getrandom"
 version = "0.2.9"
@@ -203,17 +203,17 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
@@ -386,15 +386,15 @@
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "virx_erlu_rlib"
-version = "1.1.1"
+version = "1.1.2"
 dependencies = [
  "combo_vec",
  "dubins_paths",
  "glam",
  "pyo3",
  "rand",
  "rl_ball_sym",
```

### Comparing `VirxERLU_RLib-1.1.1/PKG-INFO` & `VirxERLU_RLib-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VirxERLU-RLib
-Version: 1.1.1
+Version: 1.1.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

