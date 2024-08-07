


Sensor Fusion is the process of fusing data coming from multiple sensors.

<img src="https://i0.wp.com/semiengineering.com/wp-content/uploads/Sensor-fusion-1.png" height="60%" width="60%" />

When one or multiple sensors fail to perform accurately, sensor fusion helps in ensuring that there are no undetected objects. For example, a camera can capture the visuals around a vehicle in ideal weather conditions.

But during dense fog or heavy rainfall, the camera won’t provide sufficient data to the system. This is where radar, and to some extent, LiDAR sensors help.

Furthermore, a radar sensor may accurately show that there is a truck in the intersection where the car is waiting at a red light.

But it may not be able to generate data from a three-dimensional point of view. This is where LiDAR is needed.

## Sensor Fusion Levels

### Low-Level Fusion (Early Fusion)

In this kind of sensor fusion method, all the data coming from all sensors is fused in a single computing unit, before we begin processing it.
For example, pixels from cameras and point clouds from LiDAR sensors are fused to understand the size and shape of the object that is detected.

### Mid-Level Fusion

In mid-level fusion, objects are first detected by the individual sensors and then the algorithm fuses the data.
Generally, a Kalman filter is used to fuse this data.

The idea is to have, let’s say, a camera and a LiDAR sensor detect an obstacle individually, and then fuse the results from both to get the best estimates of position, class and velocity of the vehicle.

### High-Level Fusion (Late Fusion)

This is similar to the mid-level method, except that we implement detection as well as tracking algorithms for each individual sensor, and then fuse the results.

## Kalman Filters

https://www.thinkautonomous.ai/blog/sensor-fusion/
https://www.thinkautonomous.ai/blog/9-types-of-sensor-fusion-algorithms/


#### References
- https://medium.com/@dorlecontrols/sensor-fusion-242bc70e7332
- 



multiple sensors detect the same object may seem unnecessary in ideal scenarios, but in edge cases such as poor weather, sensor fusion is required.

