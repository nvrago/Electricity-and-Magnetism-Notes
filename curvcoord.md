# Section 1.4: Curvilinear Coordinates

## 1.4.1 Spherical Coordinates

Spherical coordinates $(r, \theta, \phi)$ are particularly useful in problems with spherical symmetry, such as the electric field of a point charge or gravitational fields. 

- **Coordinate Definitions**:
  - $r$: radial distance from the origin.
  - $\theta$: polar angle, measured from the positive $z$-axis.
  - $\phi$: azimuthal angle, measured from the positive $x$-axis in the $xy$-plane.

  The position vector $\mathbf{r}$ in spherical coordinates is expressed as $\mathbf{r} = r \mathbf{\hat{r}} = r (\sin \theta \cos \phi \mathbf{\hat{i}} + \sin \theta \sin \phi \mathbf{\hat{j}} + \cos \theta \mathbf{\hat{k}})$.

- **Differential Length Element**:

  The differential length element in spherical coordinates is $d\mathbf{l} = dr \mathbf{\hat{r}} + r d\theta \mathbf{\hat{\theta}} + r \sin \theta d\phi \mathbf{\hat{\phi}}$.

- **Differential Volume Element**:

  The volume element is $dV = r^2 \sin \theta \, dr \, d\theta \, d\phi$.

- **Surface Area Element**:
  - For a surface of constant $r$ (spherical surface): $dA = r^2 \sin \theta \, d\theta \, d\phi$.
  - For a surface of constant $\theta$ (conical surface): $dA = r \sin \theta \, dr \, d\phi$.

#### Applications:
- **Gauss's Law** in spherical coordinates simplifies calculating the electric field for spherical charge distributions. The spherical symmetry allows the electric flux to be easily computed.

<br>

## 1.4.2 Cylindrical Coordinates

Cylindrical coordinates $(\rho, \phi, z)$ are useful for problems with cylindrical symmetry, such as the field of a current-carrying wire or the electric field of a line charge.

- **Coordinate Definitions**:
  - $\rho$: radial distance from the $z$-axis.
  - $\phi$: azimuthal angle around the $z$-axis.
  - $z$: height along the $z$-axis.

  The position vector $\mathbf{r}$ in cylindrical coordinates is $\mathbf{r} = \rho \mathbf{\hat{\rho}} + z \mathbf{\hat{z}}$.

- **Differential Length Element**:

  The differential length element in cylindrical coordinates is $d\mathbf{l} = d\rho \mathbf{\hat{\rho}} + \rho d\phi \mathbf{\hat{\phi}} + dz \mathbf{\hat{z}}$.

- **Differential Volume Element**:

  The volume element is $dV = \rho \, d\rho \, d\phi \, dz$.

- **Surface Area Element**:
  - For a surface of constant $\rho$ (cylindrical surface): $dA = \rho \, d\phi \, dz$.
  - For a surface of constant $z$ (flat disk): $dA = \rho \, d\rho \, d\phi$.

#### Applications:
- **Ampere’s Law** in cylindrical coordinates helps calculate the magnetic field due to current-carrying conductors (like infinite wires). The symmetry reduces complex integrals to simple forms, making the calculation of enclosed currents straightforward.

<br>

## 1.4.3 Gradient, Divergence, and Curl in Curvilinear Coordinates

### Gradient in Spherical Coordinates
For a scalar field $f(r, \theta, \phi)$, the gradient in spherical coordinates is:

<p align="center">
$\nabla f = \frac{\partial f}{\partial r} \mathbf{\hat{r}} + \frac{1}{r} \frac{\partial f}{\partial \theta} \mathbf{\hat{\theta}} + \frac{1}{r \sin \theta} \frac{\partial f}{\partial \phi} \mathbf{\hat{\phi}}$.
</p>

### Divergence in Spherical Coordinates
The divergence of a vector field $\mathbf{A}(r, \theta, \phi)$ is:

<p align="center">
$\nabla \cdot \mathbf{A} = \frac{1}{r^2} \frac{\partial}{\partial r} (r^2 A_r) + \frac{1}{r \sin \theta} \frac{\partial}{\partial \theta} (\sin \theta A_\theta) + \frac{1}{r \sin \theta} \frac{\partial A_\phi}{\partial \phi}$.
</p>

### Curl in Spherical Coordinates
The curl of a vector field $\mathbf{A}(r, \theta, \phi)$ is:

<p align="center">
\[
\nabla \times \mathbf{A} =
\frac{1}{r \sin \theta}
\begin{vmatrix}
\mathbf{\hat{r}} & r\mathbf{\hat{\theta}} & r\sin\theta\mathbf{\hat{\phi}} \\
\frac{\partial}{\partial r} & \frac{\partial}{\partial \theta} & \frac{\partial}{\partial \phi} \\
A_r & rA_{\theta} & r\sin\theta A_{\phi}
\end{vmatrix}
=
\frac{1}{r \sin \theta} \left[
\frac{\partial}{\partial \theta} \left( A_\phi \sin \theta \right) - \frac{\partial A_\theta}{\partial \phi}
\right] \mathbf{\hat{r}} + \frac{1}{r} \left[
\frac{1}{\sin \theta} \frac{\partial A_r}{\partial \phi} - \frac{\partial}{\partial r} \left( r A_\phi \right)
\right] \mathbf{\hat{\theta}} + \frac{1}{r} \left[
\frac{\partial}{\partial r} \left( r A_\theta \right) - \frac{\partial A_r}{\partial \theta}
\right] \mathbf{\hat{\phi}}
\]
</p>

### Gradient in Cylindrical Coordinates
For a scalar function $f(\rho, \phi, z)$, the gradient is:

<p align="center">
$\nabla f = \frac{\partial f}{\partial \rho} \mathbf{\hat{\rho}} + \frac{1}{\rho} \frac{\partial f}{\partial \phi} \mathbf{\hat{\phi}} + \frac{\partial f}{\partial z} \mathbf{\hat{z}}$.
</p>

### Divergence in Cylindrical Coordinates
The divergence of a vector field $\mathbf{A}(\rho, \phi, z)$ is:

<p align="center">
$\nabla \cdot \mathbf{A} = \frac{1}{\rho} \frac{\partial}{\partial \rho} (\rho A_\rho) + \frac{1}{\rho} \frac{\partial A_\phi}{\partial \phi} + \frac{\partial A_z}{\partial z}$.
</p>

### Curl in Cylindrical Coordinates
The curl of a vector field $\mathbf{A}(\rho, \phi, z)$ is:

<p align="center">
$\nabla \times \mathbf{A} = \left( \frac{1}{\rho} \frac{\partial A_z}{\partial \phi} - \frac{\partial A_\phi}{\partial z} \right) \mathbf{\hat{\rho}} + \cdots$.
</p>

These forms are essential for solving electromagnetism problems in different curvilinear coordinates.

---

## **Additional Sections (from Landau, Feynman, and earlier editions of Griffiths)**

### **1.4.4 Generalized Curvilinear Coordinates (Landau)**

In **Landau's Electrodynamics of Continuous Media**, generalized curvilinear coordinates are used to describe more complex geometries, especially in systems like anisotropic materials (e.g., crystals) where common coordinate systems don’t suffice.

- **Mathematical Formulation**:
  In any generalized curvilinear coordinate system $(q_1, q_2, q_3)$, the basis vectors $\mathbf{e}_i$ vary with position. The differential length element is expressed as:

  $d\mathbf{l} = h_1 dq_1 \mathbf{e}_1 + h_2 dq_2 \mathbf{e}_2 + h_3 dq_3 \mathbf{e}_3$,

  where $h_i$ are the **scale factors** for the curvilinear system.

  The scale factors play a key role in determining the gradient, divergence, and curl in these coordinates. For instance, the divergence in generalized curvilinear coordinates is:

  $\nabla \cdot \mathbf{A} = \frac{1}{h_1 h_2 h_3} \left[ \frac{\partial}{\partial q_1} \left( \frac{h_2 h_3 A_1}{h_1} \right) + \frac{\partial}{\partial q_2} \left( \frac{h_1 h_3 A_2}{h_2} \right) + \frac{\partial}{\partial q_3} \left( \frac{h_1 h_2 A_3}{h_3} \right) \right]$.

#### Physical Significance:
- This generalization is crucial for studying electromagnetic fields in **anisotropic** or **inhomogeneous materials**, where the internal geometry plays a role in the behavior of fields.

#### Application in Electrodynamics:
- **Polarization** and **magnetization** in materials with complex internal structures are best treated using generalized curvilinear coordinates.

<br>

### **1.4.5 Covariant and Contravariant Basis Vectors (Landau)**

In more advanced treatments of vector calculus, it’s necessary to distinguish between **covariant** and **contravariant** components. Covariant basis vectors align with the coordinate lines, while contravariant vectors point in the direction of the coordinate axes.

- **Covariant Basis**: Denoted $\mathbf{e}_i$, these vectors are tangent to the coordinate lines.

- **Contravariant Basis**: Denoted $\mathbf{e}^i$, these vectors are normal to the surfaces of constant coordinates.

  The **covariant** and **contravariant** components of a vector $\mathbf{A}$ are related by the **metric tensor** $g_{ij}$:

  $A^i = g^{ij} A_j \quad \text{and} \quad A_i = g_{ij} A^j$.

#### Physical Significance:
This distinction is essential in **curved spaces** or **anisotropic materials** where the choice of basis vectors affects the calculation of fields.

<br>

### **1.4.6 Visualizing Curvilinear Systems (Feynman)**

In the **Feynman Lectures**, Feynman provides insights into how to **visualize curvilinear coordinate systems**. His approach emphasizes how the geometry of space changes when we switch from Cartesian coordinates to spherical or cylindrical coordinates.

- **Visualization Techniques**:
  - Feynman explains that in curvilinear systems, **grid lines** representing coordinate lines become curved, and basis vectors change with position.
  - He uses intuitive examples like imagining stretching a **rubber sheet** to understand how a vector might behave differently when we move along curvilinear coordinates.

#### Physical Insight:
Understanding how coordinate systems warp space gives deeper insight into problems like the electric potential near curved surfaces or current distributions in wires with cylindrical symmetry.

<br>

### **1.4.7 Solving Laplace’s Equation in Curvilinear Coordinates (Griffiths)**

In earlier editions of **Griffiths**, solutions to **Laplace’s equation** in curvilinear coordinates are worked out for problems involving **spherical** and **cylindrical symmetry**. 

- **Laplace’s Equation** in spherical coordinates:

  $\nabla^2 V = 0$,

  becomes separable, allowing us to solve for potentials in spherical charge distributions or cavities. Solutions are expressed in terms of **Legendre polynomials** and **spherical harmonics**.

- **Laplace’s Equation** in cylindrical coordinates:

  $\frac{1}{\rho} \frac{\partial}{\partial \rho} \left( \rho \frac{\partial V}{\partial \rho} \right) + \frac{1}{\rho^2} \frac{\partial^2 V}{\partial \phi^2} + \frac{\partial^2 V}{\partial z^2} = 0$,

  is used to describe the potential in cylindrical systems, such as the potential around an infinite line charge.

#### Applications:
- These solutions are crucial in electrostatics for determining the **electric potential** in symmetric systems and are used to solve boundary-value problems with conducting or insulating boundaries.

