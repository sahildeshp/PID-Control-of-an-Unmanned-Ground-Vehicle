# PID-Control-of-an-Unmanned-Ground-Vehicle

Implementation of a Proportional-
Integral-Derivative (PID) controller for path tracking and platooning using Lego Mindstorm EV3
Unmanned Vehicle. A PID controller is very reliable and is the most used control algorithm. The
basic idea behind a PID controller is to read a sensor, then calculate the proportional (P), integral
(I) and derivative (D) responses and sum these three components to compute the desired actuator
output [1] as shown in Figure 1. Several factors bear influence on the unmanned vehicle (UV)
when tracking the given path from point A to point B. These include variance in Reflected Light
Intensity (RLI) values due to ambient light conditions, placement of the light sensor modules, and
the stability of the designed framework for the UV.


Briefly, the main deliverables of the EV3 UV include:
1. Avoid a collision with a stationary obstacle by stopping the UV before the obstacle at the
least possible distance.
2. Implement a platooning formation by following another EV3 UV while maintaining a fixed
distance, along a straight line. A proportional (P) controller is implemented to regulate the
speed of the UV, to follow the other UV, and maintain the fixed gap.
3. Movement of the UV from source to destination along a black path silhouetted against a
white background in the least possible time with PID control used as a compensating
mechanism.


Based on the reference, error, and output signals, the designed PID controller generates appropriate
signals to the left and right motors of the UV to track the path. Three photodiodes (EE-SF5(B))
are used to detect the path and generate appropriate signals for the UV to track the path. An
ultrasonic sensor (SR04) is used to detect obstacles and/or another UV in front. The sensitivity of
the ultrasonic sensor depends on the filter design. Implementation of the timer circuit for the
ultrasonic sensor requires a careful selection of components to produce the required sampling rate.
The PID control gains are tuned accurately to control the speed of the two UV motors to travel
from point A to Point B as fast as possible by tracking the given path. The entire control algorithm
is implemented in LEGO Mindstorms EV3.
