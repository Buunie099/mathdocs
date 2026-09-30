This is a formula to determine the angle $\theta$ at which a projectile should be shot to go up over a barrier and hit a target behind it with a constant initial velocity. (Air resistance not included)

Some things we know:

$g = 9.8 \frac{m}{s^2}$

$v_0$ is a constant representing the magnitude of initial velocity.

$x_t$ is the distance from the initial position to the end of the trajectory.
$x$ is the distance from the initial position to the landing position at the elevated point.

$h$ is the height we want the projectile to land at.

$s$ is how far the barrier extends above the landing position.

$r$ is the radius of the projectile.

We can then determine that the height of the trajectory's vertex to be $d = h + s + 2r$. The reason $r$ is doubled is to provide a little wiggle room so we don't scrape the bottom of the projectile on the barrier.

Splitting $v_0$ into vector components gives us $v_{0x} = |v_0| * cos(\theta)$ and $v_{0y} = |v_0| * sin(\theta)$

Using simple kinematics equations, we can determine that $x_t = v_{0x} * 2t$ and $0 = v_{0y} + g * t$. Therefore, $\frac{x_t}{2v_{x0}} = \frac{-v_{0y}}{g}$, which turns into $gx_t = -2v_{0x}v_{0y}$. From before, $v_{0x} = |v_0| * cos(\theta)$ and $v_{0y} = |v_0| * sin(\theta)$, so we can express this like $gx_t = -2|v_0|^2cos(\theta)sin(\theta)$. But wait, there's a trig identity in here: $2cos(\theta)sin(\theta) = sin(2\theta)$. So we simplify further to get $\frac{-gx_t}{|v_0|^2} = sin(2\theta)$. Now we take the arcsine of both sides and get $\frac{arcsin(\frac{-gx_t}{|v_0|^2})}{2} = \theta$.

Now, this is a handy little formula, but it doesn't actually get the number we want because it assumes we are going to land on the *ground* at the the given $x_t$, not at our $h$.
