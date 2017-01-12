Motors
======

    Cacic is a four wheeled robot, but it has only two motors, one for each side. A drive belt transfer the rotation to the wheels.

.. image:: /img/wheelsp3at.png

[Hot] Wheels
~~~~~~~~~~~~~

    Cacic has two types of wheels, off road and indoor. The first one is for outdoor enviroment and rough terrains:

.. image:: /img/offroad.png

and the second is for flat surfaces/floors:

.. image:: /img/indoor.jpg
   :scale: 50 %

Odometry
~~~~~~~~
    `Odometry`_ is the use of data from motion sensors to estimate change in position over time. Cacic and others Pioneer-3AT has in its motors sensors (position encoders) that senses the rotation velocity then the microcontroller? or p2os? integrates this data and estimates the robot's `pose`_ relative to a starting location.

.. _Odometry: https://en.wikipedia.org/wiki/Odometry
.. _pose: https://en.wikipedia.org/wiki/Pose_(computer_vision)
