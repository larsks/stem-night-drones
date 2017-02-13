# DRONES IN SPAAAACE

This repository contains materials for my presentation at the Burbank
STEM Night on February 15, 2017.

All the software used to create this project is [FREE SOFTWARE][]
distributed under the terms of version 3 of the [GNU General Public
License][gpl].  That means that you can freely use, modify, and redistribute
this software.  The only requirement is that any modifications you
make must follow the same license.

[free software]: https://www.gnu.org/philosophy/free-sw.en.html
[gpl]: LICENSE.txt

The code I wrote for this project can be found at:

- <https://github.com/larsks/py-mpu6050>

    This is the Micropython code designed to run on an ESP 8266
    device. I'm using a Digistump [Oak][], but there are many other
    alternatives.

    It reads data from an [MPU6050][] 6DOF IMU and sends it via UDP to
    a visualization client.

- <https://github.com/larsks/py-mpu6050-client>

    This is the visualization tool, which uses a slightly modified
    demo from the [Vispy][] project to display a 3D cube that tracks
    the position information reported by the IMU.

[mpu6050]: https://www.invensense.com/products/motion-tracking/6-axis/mpu-6050/
[oak]: http://digistump.com/oak/
[vispy]: http://vispy.org/

This project depends on several other projects:

- Micropython: <https://micropython.org/>

    Micropython is a version of the Python language ported to run on
    embedded processors (such as the ESP8266).

- Vispy: <http://vispy.org/>

    Vispy is a high-performance 2D/3D visualization library for
    Python.

- i2cdevlib: <https://github.com/jrowberg/i2cdevlib>

    i2cdevlib is an Arduino library that includes code for interacting
    with the MPU6050.  While I haven't used any of the code in this
    project, I found the code to be a very useful reference.
