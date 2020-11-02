# Introduction

In robotics, two important branches are (1) state estimation and (2) control. This book focuses on state estimation.
+   The state of a robot is a set of quantities, such as position, orientation, and velocity.
+   The states can fully describe a robot's motion over time. 

# Two types of sensors
+   Interoceptive / Proprioceptive (stimuli arising within the body - velocity or acceleration)
    +   **Accelerometer** -> translation acceleration
    +   **Gyroscope** -> angular rate
    +   **Wheel odometer** -> angular rate
    +   **IMU** -> 3 linear accelerometers and 3 rate gyros
+   Exteroceptive (stimuli received by an organism from outside - position and orientation)
    +   **Cameras**
    +   Time-of-flight transmitter / receiver -> **laser**, **GPS**

# Other books
+   ***Probabilistic Robotics (2006) by Thrun***
    +   State estimation w.r.t. mapping and localization
    +   Robots operating in the 2D, horizontal plane
    +   Details of extending to 3D are not provided
+   ***Robotics, Vision, and Control (2011) by Corke***
    +   State estimation for robotics including 3D
    +   The breadth of this book necessitates that it not delve too deeply into state estimation
+   ***Many others***
    +   see the text

# Probability Preliminary

Bayes' rule, derived from joint probability definition:
$$
p(x, y) = p(x|y)p(y) = p(y|x)p(x) \rightarrow p(x|y) = \frac{p(y|x)p(x)}{p(y)} = \frac{p(y|x)p(x)}{\int p(y|x)p(x)dx}
$$
