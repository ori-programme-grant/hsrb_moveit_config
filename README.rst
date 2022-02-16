Overview
++++++++

Functions provided
--------

- This package provides the launch files that use MoveIt with the HSRB.

How to use
++++++++++

Launch files
----------------

In case you are doing a functionality test using only the Rviz simulator, start using the following launch file.
(You can even do this without a real robot or Gazebo).

.. code-block:: bash

   roslaunch hsrb_moveit_config hsrb_demo.launch

If it is the case that you want to execute commands from MoveIt directly against the actual controller of a real robot or Gazebo, start using the following launch file.

.. code-block:: bash

   roslaunch hsrb_moveit_config hsrb_demo_with_controller.launch
   
If on the robot:

.. code-block:: bash
   
   roslaunch hsrb_moveit_config hsrb_demo_with_controller.launch use_gui:=false

Then on connected display PC:

.. code-block:: bash

   roslaunch hsrb_moveit_config moveit_rviz.launch config:=true robot_name:=hsrb debug:=false

LICENSE
+++++++

This software is released under the BSD 3-Clause Clear License, see LICENSE.txt.
