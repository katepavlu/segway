
**Encoder**
Directly measures the position of the pendulum. 
Bandwidth limited to 10 Hz.

 **Gyro** 
 has higher bandwidth, however, to obtain a position, its output has to be
integrated.

**IMU (BMX055)**

Acceleration in the X, Y, and Z directions is mapped from -2 to 2 g to a signal of -1
to 1. This means that the acceleration felt due to gravity is mapped from 9.81ms−2 to
a signal of 0.5.

Rotational velocity around the X, Y, and Z axis is mapped from −500 ◦ s−1 to 500 ◦ s−1
to -1 to 1. For example, a rotation around the Z axis of 50 degrees per second, will result
in a signal of 0.1.
The sample frequency of the both accelerometer and gyro is equal to the frequency at
which the controller is running but has one sample delay.
The IMU uses the coordinate system that is defined in figure C.1. Rotations are
defined as a rotation around a certain axis. So for example a rotation around y would
mean that the segway is steering.


**Current sensor for driving the motor (AD7091R-5)**

The bandwidth  limited to 80 Hz.  
Does not measure currents below 0.2A and is not linear
below 0.3 A, see figure Figure C.2. 
After 0.3A the current (I) can be calculated from the
current sensor output (O) using the following formula:

**Complementary filter** 
https://vanhunteradams.com/Pico/ReactionWheel/Complementary_Filters.html


