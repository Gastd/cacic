ROS
===

The Robot Operating System (`ROS`_) is a flexible framework for writing robot software. It is a collection of tools, libraries, and conventions that aim to simplify the task of creating complex and robust robot behavior across a wide variety of robotic platforms. ROS has chosen as CACIC's framework because within it we can develop robotics software together with the community. Below are listed the packages that today are used and tested in the robot. To learn how to use ROS in the robot please `click here`_

.. _click here: howto.html
.. _CIC: http://www.cic.unb.br/
.. _ROS: http://www.ros.org/

Description of the Robot
~~~~~~~~~~~~~~~~~~~~~~~~
Custom package that contains the configuration files for CACIC, e.g. CAD, map, hardware configuration, hardware communication and navigation files. View the package in github_.

.. _github: https://github.com/Gastd/cacic_description

p2os stack
~~~~~~~~~~
The p2os_ is a stack, collection of packages_ that interface robot's microcontroller with the ROS system.

.. _p2os: http://wiki.ros.org/p2os
.. _packages: http://wiki.ros.org/Packages

hokuyo_node
~~~~~~~~~~~

hokuyo_node_ provide data stream from Hokuyo laser range finders.

.. _hokuyo_node: http://wiki.ros.org/hokuyo_node

sonar_viz
~~~~~~~~~

With this package is possible to view in rviz_ the sonar readings.

.. _rviz: http://wiki.ros.org/rviz

gscam
~~~~~

vcc50i_opencv
~~~~~~~~~~~~~

navigation stack
~~~~~~~~~~~~~~~~

amcl
----

gmapping
--------
