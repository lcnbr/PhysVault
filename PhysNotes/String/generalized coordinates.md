In analytical mechanics, the term **generalized coordinates** refers to the parameters that describe the configuration of the system relative to some reference configuration. These parameters must uniquely define the configuration of the system relative to the reference configuration.\[1\] This is done assuming that this can be done with a single chart. The **generalized velocities** are the time derivatives of the generalized coordinates of the system.

An example of a generalized coordinate is the angle that locates a point moving on a circle. The adjective "generalized" distinguishes these parameters from the traditional use of the term coordinate to refer to Cartesian coordinates: for example, describing the location of the point on the circle using x and y coordinates.

Although there may be many choices for generalized coordinates for a physical system, parameters that are convenient are usually selected for the specification of the configuration of the system and which make the solution of its equations of motion easier. If these parameters are independent of one another, the number of independent generalized coordinates is defined by the number of degrees of freedom of the system.\[2\]\[3\]

Generalized coordinates are paired with generalized momenta to provide [[canonical coordinates]] on phase space.

## Constraints and degrees of freedom

![](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d6/Generalized_coordinates_open_straight_path_2d_1df.svg/153px-Generalized_coordinates_open_straight_path_2d_1df.svg.png)

Open straight path

![](https://upload.wikimedia.org/wikipedia/commons/thumb/0/00/Generalized_coordinates_open_curved_path_2d_1df.svg/167px-Generalized_coordinates_open_curved_path_2d_1df.svg.png)

Open curved path _F_(_x_, _y_) = 0

![](https://upload.wikimedia.org/wikipedia/commons/thumb/0/01/Generalized_coordinates_closed_path_2d_1df.svg/155px-Generalized_coordinates_closed_path_2d_1df.svg.png)

Closed curved path _C_(_x_, _y_) = 0

One generalized coordinate (one degree of freedom) on paths in 2D. Only one generalized coordinate is needed to uniquely specify positions on the curve. In these examples, that variable is either arc length _s_ or angle _θ_. Having both of the Cartesian coordinates (_x_, _y_) are unnecessary since either _x_ or _y_ is related to the other by the equations of the curves. They can also be parameterized by _s_ or _θ_.

![](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3f/Non_generalized_coordinates_open_curved_path_2d_1df.svg/150px-Non_generalized_coordinates_open_curved_path_2d_1df.svg.png)

Open curved path _F_(_x_, _y_) = 0. Multiple intersections of radius with path.

![](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c2/Non_generalized_coordinates_closed_curved_path_2d_1df.svg/164px-Non_generalized_coordinates_closed_curved_path_2d_1df.svg.png)

Closed curved path _C_(_x_, _y_) = 0. Self-intersection of path.

The arc length _s_ along the curve is a legitimate generalized coordinate since the position is uniquely determined, but the angle _θ_ is not since there are multiple positions for a single value of _θ_.

Generalized coordinates are usually selected to provide the minimum number of independent coordinates that define the configuration of a system, which simplifies the formulation of Lagrange's equations of motion. However, it can also occur that a useful set of generalized coordinates may be _dependent_, which means that they are related by one or more constraint equations.

### Holonomic constraints

![](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d3/Generalized_coordinates_open_curved_path_3d_2df.svg/186px-Generalized_coordinates_open_curved_path_3d_2df.svg.png)

Open curved surface _F_(_x_, _y_, _z_) = 0

![](https://upload.wikimedia.org/wikipedia/commons/thumb/8/86/Generalized_coordinates_closed_curved_path_3d_2df.svg/198px-Generalized_coordinates_closed_curved_path_3d_2df.svg.png)

Closed curved surface _S_(_x_, _y_, _z_) = 0

Two generalized coordinates, two degrees of freedom, on curved surfaces in 3d. Only two numbers (_u_, _v_) are needed to specify the points on the curve, one possibility is shown for each case. The full three Cartesian coordinates (_x_, _y_, _z_) are not necessary because any two determines the third according to the equations of the curves.

For a system of _N_ particles in 3D real coordinate space, the position vector of each particle can be written as a 3-tuple in Cartesian coordinates:

![\mathbf{r}_1 = (x_1,y_1,z_1) \,, \quad \mathbf{r}_2 = (x_2,y_2,z_2) \,, \ldots \,, \mathbf{r}_N = (x_N,y_N,z_N)\,. ](https://wikimedia.org/api/rest_v1/media/math/render/svg/8657a5c0c39f33e15ec6d9cfee9ba5f341cd6748)

Any of the position vectors can be denoted **r**_k_ where _k_ = 1, 2, ..., _N_ labels the particles. A _holonomic constraint_ is a _constraint equation_ of the form for particle _k_\[4\]\[nb 1\]

![f(\mathbf{r}_k, t) = 0](https://wikimedia.org/api/rest_v1/media/math/render/svg/17bcd6d78bd705e15de85609cdbdc9b0ec91a895)

which connects all the 3 spatial coordinates of that particle together, so they are not independent. The constraint may change with time, so time _t_ will appear explicitly in the constraint equations. At any instant of time, any one coordinate will be determined from the other coordinates, e.g. if _xk_ and _zk_ are given, then so is _yk_. One constraint equation counts as _one_ constraint. If there are _C_ constraints, each has an equation, so there will be _C_ constraint equations. There is not necessarily one constraint equation for each particle, and if there are no constraints on the system then there are no constraint equations.

So far, the configuration of the system is defined by 3_N_ quantities, but _C_ coordinates can be eliminated, one coordinate from each constraint equation. The number of independent coordinates is _n_ = 3_N_ − _C_. (In _D_ dimensions, the original configuration would need _ND_ coordinates, and the reduction by constraints means _n_ = _ND_ − _C_). It is ideal to use the minimum number of coordinates needed to define the configuration of the entire system, while taking advantage of the constraints on the system. These quantities are known as **generalized coordinates** in this context, denoted _qj_(_t_). It is convenient to collect them into an _n_\-tuple

![\mathbf{q}(t) = (q_1(t), q_2(t), \ldots, q_n(t)) ](https://wikimedia.org/api/rest_v1/media/math/render/svg/35b6840aee2d9059d313fd7185b087caaaa4c933)

which is a point in the _configuration space_ of the system. They are all independent of one other, and each is a function of time. Geometrically they can be lengths along straight lines, or arc lengths along curves, or angles; not necessarily Cartesian coordinates or other standard orthogonal coordinates. There is one for each degree of freedom, so the number of generalized coordinates equals the number of degrees of freedom, _n_. A degree of freedom corresponds to one quantity that changes the configuration of the system, for example the angle of a pendulum, or the arc length traversed by a bead along a wire.

If it is possible to find from the constraints as many independent variables as there are degrees of freedom, these can be used as generalized coordinates.\[5\] The position vector **r**_k_ of particle _k_ is a function of all the _n_ generalized coordinates (and, through them, of time),\[6\]\[7\]\[8\]\[5\]\[nb 2\]

![{\displaystyle \mathbf {r} _{k}=\mathbf {r} _{k}(\mathbf {q} (t))\,,}](https://wikimedia.org/api/rest_v1/media/math/render/svg/5b494f7554b44238321a4940ee1b235e2f8621d2)

and the generalized coordinates can be thought of as parameters associated with the constraint.

The corresponding time derivatives of **q** are the generalized velocities,

![\dot{\mathbf{q}} = \frac{d\mathbf{q}}{dt} = (\dot{q}_1(t), \dot{q}_2(t), \ldots, \dot{q}_n(t)) ](https://wikimedia.org/api/rest_v1/media/math/render/svg/4964eb614f4e21ef7015ac3ed36c7ebf0f2db502)

(each dot over a quantity indicates one time derivative). The velocity vector **v**_k_ is the total derivative of **r**_k_ with respect to time

![{\displaystyle \mathbf {v} _{k}={\dot {\mathbf {r} }}_{k}={\frac {d\mathbf {r} _{k}}{dt}}=\sum _{j=1}^{n}{\frac {\partial \mathbf {r} _{k}}{\partial q_{j}}}{\dot {q}}_{j}\,.}](https://wikimedia.org/api/rest_v1/media/math/render/svg/fe3a69280ed0ca5245441c3fb34e5995c2b4fc02)

and so generally depends on the generalized velocities and coordinates. Since we are free to specify the initial values of the generalized coordinates and velocities separately, the generalized coordinates _qj_ and velocities _dqj_/_dt_ can be treated as _independent variables_.

### Non-holonomic constraints

A mechanical system can involve constraints on both the generalized coordinates and their derivatives. Constraints of this type are known as non-holonomic. First-order non-holonomic constraints have the form

![g(\mathbf{q}, \dot{\mathbf{q}}, t) = 0\,,](https://wikimedia.org/api/rest_v1/media/math/render/svg/fada4a49c2c2585de11aa423da7770f2547a4de1)

An example of such a constraint is a rolling wheel or knife-edge that constrains the direction of the velocity vector. Non-holonomic constraints can also involve next-order derivatives such as generalized accelerations.

## Physical quantities in generalized coordinates

### Kinetic energy

The total kinetic energy of the system is the energy of the system's motion, defined as\[9\]

![T = \frac {1}{2} \sum_{k=1}^N m_k \dot{\mathbf{r}}_k \cdot \dot{\mathbf{r}}_k\,,](https://wikimedia.org/api/rest_v1/media/math/render/svg/c3b803ede6c3a48e07e66ef7283021daea2ae6fb)

in which · is the dot product. The kinetic energy is a function only of the velocities **v**_k_, not the coordinates **r**_k_ themselves. By contrast an important observation is\[10\]

![{\displaystyle {\dot {\mathbf {r} }}_{k}\cdot {\dot {\mathbf {r} }}_{k}=\sum _{i,j=1}^{n}\left({\frac {\partial \mathbf {r} _{k}}{\partial q_{i}}}\cdot {\frac {\partial \mathbf {r} _{k}}{\partial q_{j}}}\right){\dot {q}}_{i}{\dot {q}}_{j},}](https://wikimedia.org/api/rest_v1/media/math/render/svg/7c728886df572bc2d4b93654a3da06fdb4e4882c)

which illustrates the kinetic energy is in general a function of the generalized velocities, coordinates, and time if the constraints also vary with time, so _T_ = _T_(**q**, _d_**q**/_dt_, _t_).

In the case the constraints on the particles are time-independent, then all partial derivatives with respect to time are zero, and the kinetic energy is a homogeneous function of degree 2 in the generalized velocities.

Still for the time-independent case, this expression is equivalent to taking the line element squared of the trajectory for particle _k_,

![ds_k^2 = d\mathbf{r}_k\cdot d\mathbf{r}_k = \sum_{i,j=1}^n \left(\frac{\partial \mathbf{r}_k}{\partial q_i}\cdot\frac{\partial \mathbf{r}_k}{\partial q_j}\right) dq_i dq_j \,,](https://wikimedia.org/api/rest_v1/media/math/render/svg/8bdb973c02a59a6c81ddc363b74c74b6cdfe7b54)

and dividing by the square differential in time, _dt_2, to obtain the velocity squared of particle _k_. Thus for time-independent constraints it is sufficient to know the line element to quickly obtain the kinetic energy of particles and hence the Lagrangian.\[11\]

It is instructive to see the various cases of polar coordinates in 2d and 3d, owing to their frequent appearance. In 2d polar coordinates (_r_, _θ_),

![\left(\frac{ds}{dt}\right)^2 = \dot{r}^2 + r^2\dot{\theta}^2 \,,](https://wikimedia.org/api/rest_v1/media/math/render/svg/9641c8444599cf5018fd5a88585f6d755182b691)

in 3d cylindrical coordinates (_r_, _θ_, _z_),

![\left(\frac{ds}{dt}\right)^2 = \dot{r}^2 + r^2\dot{\theta}^2 + \dot{z}^2 \,,](https://wikimedia.org/api/rest_v1/media/math/render/svg/dacd2a38c324259a7154082dcb460776bd4537b2)

in 3d spherical coordinates (_r_, _θ_, _φ_),

![\left(\frac{ds}{dt}\right)^2 = \dot{r}^2+r^2\dot{\theta}^2 +r^2\sin^2\theta \, \dot{\varphi}^2 \,.](https://wikimedia.org/api/rest_v1/media/math/render/svg/edcbc643834325a246ca0841ed38cc8ad04ad0c6)

### Generalized momentum

The _generalized momentum_ "canonically conjugate to" the coordinate _qi_ is defined by

![p_{i}={\frac {\partial L}{\partial {\dot {q}}_{i}}}.](https://wikimedia.org/api/rest_v1/media/math/render/svg/732cdc7f806d3627bd7b414c709a7d1d5e9f20f3)

If the Lagrangian _L_ does _not_ depend on some coordinate _qi_, then it follows from the Euler–Lagrange equations that the corresponding generalized momentum will be a conserved quantity, because the time derivative is zero implying the momentum is a constant of the motion;

![{\dot {p}}_{i}={\frac {d}{dt}}{\frac {\partial L}{\partial {\dot {q}}_{i}}}={\frac {\partial L}{\partial q_{i}}}=0\,.](https://wikimedia.org/api/rest_v1/media/math/render/svg/fde9185ebe680e08764b26a37545f6973b21eddb)

