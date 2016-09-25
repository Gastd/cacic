Camera
======

Cacic has a `PTZ Camera`_, Canon VC C50i

.. _PTZ Camera: https://en.wikipedia.org/wiki/Pan%E2%80%93tilt%E2%80%93zoom_camera

.. image:: /img/canon_vc-c50i_med.jpg

Main Especs
~~~~~~~~~~~

- Resolution: 640x480
- Zoom: up to 26x optical
- Pan/Tilt range: 200-degree pan range, 120-degree tilt range
- Pan/Tilt speed: up to 90-degrees Pan and 70-degrees Tilt per second 
- Format: NTSC
- Power Supply: 13 VDC
- Stream Interface: RCA-BNC Cable
- Control Interface: Custom multiconnector with terminals S-VIDEO OUT, RS232 OUT and RS232 IN
- Framegrabber: `Sensoray 311`_

.. note::
    
    There is wireless controller that came with camera, it work but is not used.

.. _Sensoray 311: camera.html#framegrabber


Linux Drivers
~~~~~~~~~~~~~

For the Camera
--------------
   The cameras's stream can be retrived with OpenCV using Video4Linux. Checkout this code.


For the Pan-Tilt-Zoom 
---------------------
   Camera's PTZ can be controlled with `P2OS`_ package in `ROS`_

.. _P2OS: p2os.tml
.. _ROS: ros.html

Framegrabber
~~~~~~~~~~~~
Sensoray 311 with interface PC104+, manufactured by `Sensoray`_

.. _Sensoray: Sensoray.com

.. image:: /img/Sensoray_311_Framegrabber_PC104.jpg

Linux 2.4.x Driver
   Use built in 'bttv' module with parameter: card=73

Linux 2.6.x Driver
   Use v4l with parameter: card=73

Troublehooting
~~~~~~~~~~~~~~

Blue or black screen when retriving frame using OpenCV
------------------------------------------------------
    1. Check the camera's LED
        The camera is switched off, start P2OS to switch the camera on.
    2. `Check the power`_
        If the LED is off, maybe the power to the camera is switched off. Press the AUX 1 and AUX 2 buttons on the robot's panel.

.. _Check the power: http://robots.mobilerobots.com/wiki/Why_doesn%27t_my_camera_turn_on%3F

Blue or black screen when retriving frame using another software
----------------------------------------------------------------
    Same for OpenCV, check the section above.

Scramble image
--------------

    1. Switch v4l to retrieve the input with NTSC format
        Open the terminal and try

        .. code-block:: bash

            $ v4l2-ctl -s ntsc


    2. Using gscam and ROS?
        Set enviroment variable GSCAM_CONFIG="v4l2src ! video/x-raw-yuv, width=320, height=240 ! ffmpegcolorspace"

.. todo:change width and height


More trouble?
-------------
    Check `here`_.

.. _here: http://robots.mobilerobots.com/wiki/Capturing_Video#Troubleshooting

IF YOU ARE TR00 FUCKING HARD
~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    Maybe you want to use `it`_.

.. _it: https://raw.githubusercontent.com/Gastd/cacic/master/sample_code/V4l2capture.c
