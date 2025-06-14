^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package swri_transform_util
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

2.15.4 (2025-02-26)
-------------------
* Removing version check on Kinetic for C++ standard (`#760 <https://github.com/swri-robotics/marti_common/issues/760>`_)
* Contributors: David Anthony

2.15.3 (2025-02-21)
-------------------
* Updating for New Proj Versions (`#733 <https://github.com/swri-robotics/marti_common/issues/733>`_)
  Updated using changes from the ros2-devel branch to support new PROJ versions.
* Increase minimum CMake version to 3.16 to satisfy the compatiblity check in newer CMake versions (`#732 <https://github.com/swri-robotics/marti_common/issues/732>`_)
  Co-authored-by: Daniel D'Souza <daniel.dsouza@swri.org>
* Adding Adelaide test case for UTM coordinate conversion (`#724 <https://github.com/swri-robotics/marti_common/issues/724>`_)
* Contributors: Daniel D'Souza, David Anthony

2.15.2 (2022-09-01)
-------------------

2.14.2 (2020-09-09)
-------------------
* stamp local_xy_origin message picked from list with now() (`#600 <https://github.com/swri-robotics/marti_common/issues/600>`_)
* Contributors: Daniel D'Souza, P. J. Reed

2.14.1 (2020-08-18)
-------------------
* Fix 90 deg transform (`#598 <https://github.com/swri-robotics/marti_common/issues/598>`_)
* Contributors: Alex Youngs

2.14.0 (2020-07-15)
-------------------
* Added python support for wgs84 transforms (`#595 <https://github.com/swri-robotics/marti_common/issues/595>`_)
* Contributors: Alex Youngs

2.13.7 (2020-06-26)
-------------------
* Improve object transformer to take into account the pose of the object (`#589 <https://github.com/swri-robotics/marti_common/issues/589>`_)
* Contributors: Matthew Bries

2.13.6 (2020-06-17)
-------------------
* Update catkin dependencies (`#588 <https://github.com/swri-robotics/marti_common/issues/588>`_)
* Contributors: P. J. Reed

2.13.5 (2020-06-17)
-------------------

2.13.4 (2020-06-16)
-------------------
* Clean up Boost usage (`#584 <https://github.com/swri-robotics/marti_common/issues/584>`_)
* Contributors: P. J. Reed

2.13.3 (2020-06-12)
-------------------
* Use setuptools instead of distutils (`#583 <https://github.com/swri-robotics/marti_common/issues/583>`_)
* Bump minimum cmake version
* Contributors: Shane Loretz, P. J. Reed

2.13.2 (2020-06-10)
-------------------
* Support ROS Noetic (`#581 <https://github.com/swri-robotics/marti_common/issues/581>`_)
* Contributors: P. J. Reed

2.13.1 (2020-05-21)
-------------------

2.13.0 (2020-05-13)
-------------------
* Fix build with Boost >=1.69 (`#574 <https://github.com/swri-robotics/marti_common/issues/574>`_)
* Contributors: Ben Wolsieffer

2.12.0 (2020-03-25)
-------------------
* Suppress auto_ptr warnings (`#570 <https://github.com/swri-robotics/marti_common/issues/570>`_)
* Contributors: P. J. Reed

2.11.0 (2019-11-13)
-------------------
* Add a nodelet that transforms ObstacleArrays
* Install gps_transform_publisher node (`#551 <https://github.com/pjreed/marti_common/issues/551>`_)
* Contributors: Matthew, P. J. Reed

2.10.0 (2019-09-04)
-------------------
* Support in initialize_origin.py specifying custom ROS topic in parameter (`#544 <https://github.com/swri-robotics/marti_common/issues/544>`_)
* Fix get relative transform (`#546 <https://github.com/swri-robotics/marti_common/issues/546>`_)
* Contributors: Arkady Shapkin, Matthew

2.9.0 (2019-05-23)
------------------

2.8.0 (2019-02-06)
------------------
* Reduce the number of local_xy subscribers from 3 per transform manager to 1 (`#537 <https://github.com/swri-robotics/marti_common/issues/537>`_)
* Add dynamic parameters (`#532 <https://github.com/swri-robotics/marti_common/issues/532>`_)
* Contributors: Matthew

2.7.3 (2019-01-03)
------------------

2.7.2 (2018-12-20)
------------------
* Fix the unit test that intermittently breaks (`#534 <https://github.com/swri-robotics/marti_common/issues/534>`_)
* Contributors: P. J. Reed

2.7.1 (2018-12-14)
------------------

2.7.0 (2018-12-04)
------------------

2.6.0 (2018-11-03)
------------------

2.5.0 (2018-10-12)
------------------

2.4.0 (2018-10-09)
------------------
* Handle invalid fixes properly (`#519 <https://github.com/swri-robotics/marti_common/issues/519>`_)
* Contributors: P. J. Reed

2.3.0 (2018-05-25)
------------------
* Initialize transform timestamp to 0 instead of ros::Time::now() (`#515 <https://github.com/swri-robotics/marti_common/issues/515>`_)
* Contributors: Marc Alban

2.2.1 (2018-05-11)
------------------
* Support ROS Melodic (`#514 <https://github.com/swri-robotics/marti_common/issues/514>`_)
* Contributors: P. J. Reed

2.2.0 (2018-02-12)
------------------
* Add gps_transform_publisher. (`#509 <https://github.com/swri-robotics/marti_common/issues/509>`_)
* Contributors: Marc Alban

2.1.0 (2018-01-26)
------------------

2.0.0 (2017-12-18)
------------------
* expose TransformManager::LocalXyUtil() and LocalXyWgs84Util::ResetInitialization() (`#501 <https://github.com/swri-robotics/marti_common/issues/501>`_)
* Complete rewrite of initialize_origin.py (`#491 <https://github.com/swri-robotics/marti_common/issues/491>`_)
* Normalize TF frames before comparisons. (`#492 <https://github.com/swri-robotics/marti_common/issues/492>`_)
* Add new methods that expose the frame timeout. (`#498 <https://github.com/swri-robotics/marti_common/issues/498>`_)
* Use pkgconfig to include libproj in swri_transform_util
* Contributors: Davide Faconti, Edward Venator, P. J. Reed

1.2.0 (2017-10-13)
------------------

1.1.0 (2017-08-31)
------------------
* Revert "Remove nodelet_plugins.xml from CMakeLists.txt" (`#475 <https://github.com/pjreed/marti_common/issues/475>`_)
* Document swri_transform_util (`#456 <https://github.com/pjreed/marti_common/issues/456>`_)
* Contributors: Edward Venator, Marc Alban, P. J. Reed

1.0.0 (2017-08-02)
------------------
* Increase delay before running tests.
* Integrate transformers as static classes instead of plug-ins.
* Add inverse transform implementation to transforms. (`#464 <https://github.com/evenator/marti_common/issues/464>`_)
* Add tests for initialize_origin.py script (`#457 <https://github.com/evenator/marti_common/issues/457>`_)
* Contributors: Edward Venator, Marc Alban

0.3.0 (2017-06-20)
------------------
* Merge together the indigo, jade, and kinetic branches (`#443 <https://github.com/pjreed/marti_common/issues/443>`_)
* Fix dynamic reconfigure in dynamic_publisher (closes issue `#448 <https://github.com/pjreed/marti_common/issues/448>`_).
* Contributors: Elliot Johnson, P. J. Reed

0.2.4 (2017-04-11)
------------------
* Ignore invalid fixes
  Fixes `#431 <https://github.com/swri-robotics/marti_common/issues/431>`_.
* Remove unused gps_common dependency (`#422 <https://github.com/swri-robotics/marti_common/issues/422>`_)
  Fix `#421 <https://github.com/swri-robotics/marti_common/issues/421>`_ by removing gps_common from the swri_transform_util CMakeLists.txt in kinetic.
* Simplify dynamic reconfigure usage.
* Add nodelet for publishing a dynamically reconfigurable TF transform.
* Contributors: Edward Venator, Marc Alban, P. J. Reed

0.2.3 (2016-12-09)
------------------

0.2.2 (2016-12-07)
------------------
* Migrated OpenCV to 3.1 (default in Kinetic)
* Contributors: Brian Holt

0.2.1 (2016-10-23)
------------------
* Improve georeferencing warnings.
* Contributors: Marc Alban

0.2.0 (2016-06-21)
------------------

0.1.5 (2016-05-13)
------------------

0.1.4 (2016-05-12)
------------------
* Add great circle distance method for tf::Vector3 type.
* Fixed compile error when ros-indigo-opencv3 is installed (`#307 <https://github.com/evenator/marti_common/issues/307>`_)
* Contributors: Kim Mathiassen, Marc Alban

0.1.3 (2016-03-04)
------------------
* Fixes initialize_origin.py diagnostic reporting a warning that the
  origin is not automatic when it is.
* Adds transform publisher to initialize_origin.py that publishes an
  identity transform from the local_xy_frame to an anonymous unused
  frame.  In doing so, the local_xy_frame will show up
  in the /tf tree without any additional nodes running so that
  TransformManager can properly transform between /wgs84 and /map.
  This change should not interfere with any existing systems.
* Expands some of the TransformManager warnings to be more
  informative.  This is to reduce the impact of common problems that we
  run into when setting up a new environment by making it easier to
  distinguish the exact nature of the error, as well as provide
  suggestions when appropriate.
  In particular, this fixes the misleading
  "No transfomer from /wgs84 to /map" error and upgrades a warning
  about null pointers to an error.
* Contributors: Elliot Johnson

0.1.2 (2016-01-06)
------------------
* Account for non-zero reference angles when calculating orientations to and from WGS84.
* Support arbitrary local_xy reference angles.
  * The reference heading has been renamed to reference angle.
  * It's not recommended to set a non-zero reference angle.
  * A parameter is provided to ignore the reference heading for backwards compatibility.
* Fix backwards compatibility issue with swri_yaml_cpp call.
* Contributors: Kris Kozak, Marc Alban

0.1.1 (2015-11-17)
------------------
* Adds a GetTF method to transform_util::Transform.
* Installing the initialize_origin.py node.
* Add extension type (e.g. png) in geo file
* Contributors: Edward Venator, P. J. Reed, Vincent Rousseau

0.1.0 (2015-09-29)
------------------
* Updates lot_lon_tf_echo to use geometry_msgs/PoseStamped.
  See issue `#246 <https://github.com/evenator/marti_common/issues/246>`__
* Removes dependency on gps_common
  The gps_common package was removed in ROS Jade, so a different message
  type is needed for the local XY origin message. (Issue `#246 <https://github.com/swri-robotics/marti_common/issues/246>`__).
  This replaces the gps_common/GPSFix message with a
  geometry_msgs/PoseStamped message. The latitude is stored in
  pose.position.y, the longitude is stored in pose.position.x, and the
  altitude is stored in pose.position.z. As before, the local xy frame is
  fixed in rotation such that the Z axis points away from the center of
  the Earth and the Y axis points north. However, the choice of
  geometry_msgs/PoseStamped allows for headings to be added in the future.
* Refactors initialize origin and fixes a bug.
* Contributors: Edward Venator

0.0.14 (2017-04-11)
-------------------
* Merge pull request `#435 <https://github.com/swri-robotics/marti_common/issues/435>`_ from swri-robotics/initialize-origin-license
  Fix whitespace and license in initialize_origin.py
* Fix whitespace and license in initialize_origin.py
  Replace "all rights reserved" with standard BSD 3-clause text and remove trailing whitespace in initialize_origin.py
* Fixes `#431 <https://github.com/swri-robotics/marti_common/issues/431>`_

0.0.13 (2016-10-23)
-------------------

0.0.12 (2016-08-14)
-------------------
* Add explicit getOrientation function for Utm transformer
* Improve georeferencing warnings.
* Contributors: Jason Gassaway, Marc Alban

0.0.11 (2016-05-13)
-------------------

0.0.10 (2016-05-12)
-------------------

0.0.9 (2016-03-04)
------------------

0.0.8 (2016-01-06)
------------------
* Accounts for non-zero reference angles when calculating orientations to and from WGS84.
* Publishes origin with east orientation (0 yaw) by default.
* Supports arbitrary local_xy reference angles.
  * The reference heading is renamed to reference angle.
  * It's not recommended to set a non-zero reference angle.
  * Adds a parameter to ignore the reference heading for backwards compatibility.
* Fixes backwards compatibility issue with swri_yaml_cpp call.
* Contributors: Kris Kozak, Marc Alban

0.0.7 (2015-11-18)
------------------

0.0.6 (2015-11-17)
------------------
* Adds a GetTF method to transform_util::Transform.
* Properly installs the initialize_origin.py node.
* Add extension type (e.g. png) in geo file
* Contributors: Edward Venator, P. J. Reed, Vincent Rousseau

0.0.5 (2015-09-27)
------------------

0.0.4 (2015-09-27)
------------------
* Fixes missing dependencies. `#239 <https://github.com/swri-robotics/marti_common/issues/239>`_.
* Contributors: Ed Venator

0.0.3 (2015-09-26)
------------------

0.0.2 (2015-09-25)
------------------
* Renames yaml_util to swri_yaml_util. Refs `#231 <https://github.com/swri-robotics/marti_common/issues/231>`_.
* Renames transform_util to swri_transform_util. Refs `#231 <https://github.com/swri-robotics/marti_common/issues/231>`_.
* Contributors: Edward Venator

0.0.1 (2015-09-25)
------------------
