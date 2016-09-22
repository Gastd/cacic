Laser
=====

Cacic has Scanning Laser Range Finder, Hokuyo UTM-30LX

.. image:: /img/hokuyo.jpg

Image credit: `RobotShop`_

.. _RobotShop: http://www.robotshop.com/en/hokuyo-utm-03lx-laser-scanning-rangefinder.html

Laser Especs
~~~~~~~~~~~~
* Supply Voltage: 12VDC +- 10%
* Supply Current: 1.0 MAX, 0.7 NORMAL
* Detection Range: 0.1 ~ 30m
* Measurement Resolution: 0.1~10m: σ < 10mm, 10~30: σ < 30mm
* Scan Angle: 270°
* Angular resolution: 0.25° (360°/1440)
* Scan Speed: 25ms
* Interface: USB 2.0

Driver
~~~~~~
    The comunication with the device is provided by a `ROS node`_, go to `How to use the laser`_ for more details.

.. _ROS node: http://wiki.ros.org/hokuyo_node

.. _How to use the laser: howto.html#using-the-laser

.. note::
    
    The `urg_node`_ is a newer driver and fully `REP 138`_ compliant, maybe in the future we will use it.


.. _urg_node: http://wiki.ros.org/urg_node

.. _REP 138: http://www.ros.org/reps/rep-0138.html

DC-DC Power Supply
~~~~~~~~~~~~~~~~~~
    The Laser has a custom circuit board to supply voltage and current with highly precision. The project was made in Frienting? by a nordic gnome, you can view and modify the project in `whatever`_.

.. _whatever: idontknow.html
