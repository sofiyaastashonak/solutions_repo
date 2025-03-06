# Problem 1
# Investigating the Range as a Function of the Angle of Projection

## 1. Theoretical Background

To study the motion of a projectile, i start from the basic equations of projectile motion. In the absence of air resistance, the motion of a projectile is determined by the following kinematic equations:

- **Horizontal motion:**
$$x(t) = v_0 \cdot \cos(\theta) \cdot t$$
  where:
  - $x(t)$ is the horizontal position,
  - $v_0$ is the initial velocity,
  - $\theta$ is the angle of launch (in radians),
  - $t$ is the time elapsed.

- **Vertical motion:**
$$y(t) = v_0 \cdot \sin(\theta) \cdot t - \frac{1}{2} g \cdot t^2$$
  where:
  - $y(t)$ is the vertical position,
  - $g$ is the acceleration due to gravity (approximately $9.81 \, \text{m/s}^2$.

By combining these equations, we can determine the **range** (horizontal distance traveled) and **maximum height** of the projectile.

## 2. Problem Setup and Solution Family

We aim to find how the **horizontal range** of the projectile depends on the launch angle and other parameters. The range can be found by determining the time of flight and the horizontal displacement at that time. The time of flight $t_{\text{flight}}$ is given by:

$$
t_{\text{flight}} = \frac{2 v_0 \sin(\theta)}{g}
$$

Substituting this into the equation for $x(t)$, we get the horizontal range:

$$
R = v_0 \cos(\theta) \cdot t_{\text{flight}} = \frac{v_0^2 \sin(2\theta)}{g}
$$

This equation shows that the range is dependent on the initial velocity $v_0$, the launch angle $\theta\ $, and the gravitational acceleration $g$. The optimal launch angle for maximum range is 45°, as $\sin(2 \cdot 45^\circ) = 1$.

For various values of the launch angle $\theta\ $, we can plot the trajectory of the projectile and observe how the range and maximum height change with different initial speeds and angles.
