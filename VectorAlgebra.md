# Section 1.1: Vector Algebra

## 1.1.1 Vector Operations

Vectors are quantities defined by both a magnitude and a direction, fundamental in electrodynamics for describing physical quantities like fields, forces, and velocities. The algebraic operations involving vectors are critical for understanding more complex topics like electric and magnetic fields. The following are key operations on vectors.

### Vector Addition
If **A** and **B** are vectors:
\[
\mathbf{C} = \mathbf{A} + \mathbf{B}
\]
Geometrically, this corresponds to placing vectors head to tail and drawing the resultant vector from the tail of the first to the head of the second.

#### Insight from Feynman:
Feynman points out that vector addition is a purely geometric process, and the concept of directionality, while often abstract, is physically realized in fields like the electric field, where the sum of vectors corresponds to the superposition principle—**the total field at a point is the vector sum of all contributions**【12†source】.

### Scalar Multiplication
Scaling a vector by a scalar \( \lambda \):
\[
\mathbf{B} = \lambda \mathbf{A}
\]
This changes the magnitude of the vector but not the direction (unless \( \lambda \) is negative, which reverses the direction). This operation is crucial in both the electric field and magnetic field analysis when dealing with magnitudes of forces or fields.

### Dot Product
The dot product (or scalar product) of two vectors **A** and **B** is defined as:
\[
\mathbf{A} \cdot \mathbf{B} = AB \cos \theta
\]
Where \( \theta \) is the angle between **A** and **B**. This operation results in a scalar and is **commutative**:
\[
\mathbf{A} \cdot \mathbf{B} = \mathbf{B} \cdot \mathbf{A}
\]
The dot product is essential in electrodynamics, particularly in expressing the work done by a force over a distance or in calculating the projection of one vector onto another.

#### Physical Significance in Electrodynamics:
In the context of electric fields, the dot product is used to compute the flux of a field through a surface. The electric flux \( \Phi \) through a surface \( S \) is given by:
\[
\Phi = \int_S \mathbf{E} \cdot d\mathbf{A}
\]
where \( d\mathbf{A} \) is a surface element vector normal to the surface.

### Cross Product
The cross product (or vector product) results in a vector that is **perpendicular** to the plane defined by **A** and **B**:
\[
\mathbf{A} \times \mathbf{B} = AB \sin \theta \, \mathbf{\hat{n}}
\]
Where \( \mathbf{\hat{n}} \) is the unit vector perpendicular to the plane. The direction of \( \mathbf{\hat{n}} \) is determined by the right-hand rule. This operation is **not commutative**:
\[
\mathbf{A} \times \mathbf{B} = -(\mathbf{B} \times \mathbf{A})
\]
This product is fundamental in calculating the torque exerted by a force and in the magnetic force on a moving charge (Lorentz force):
\[
\mathbf{F} = q\mathbf{v} \times \mathbf{B}
\]

#### Insight from Landau:
Landau emphasizes that the cross product plays a central role in the **pseudovector** nature of magnetic fields. In a medium, the cross product helps describe macroscopic magnetization and the forces it experiences, especially in **magnetized materials**【12†source】. Additionally, the cross product formalism underpins the rotational properties of vector fields, such as the curl of the electric and magnetic fields in Maxwell's equations.

#### Further from Feynman:
Feynman highlights the geometric interpretation of the cross product and its deep connection to physical phenomena like the torque and magnetic moment, reinforcing the need to understand both its magnitude and direction. The cross product reveals the inherent chirality (handedness) in physical laws like the Lorentz force【9†source】.

## 1.1.2 Vector Algebra: Component Form

Vectors are often expressed in terms of their components along the Cartesian axes. For a vector **A**, we can write:
\[
\mathbf{A} = A_x \mathbf{\hat{i}} + A_y \mathbf{\hat{j}} + A_z \mathbf{\hat{k}}
\]
Where \( \mathbf{\hat{i}}, \mathbf{\hat{j}}, \mathbf{\hat{k}} \) are the unit vectors along the \( x \), \( y \), and \( z \) axes, respectively. The magnitude of the vector is given by:
\[
|\mathbf{A}| = \sqrt{A_x^2 + A_y^2 + A_z^2}
\]
This form simplifies vector operations like the dot and cross product, which can be calculated component-wise.

### Dot Product in Component Form
For vectors \( \mathbf{A} = A_x \mathbf{\hat{i}} + A_y \mathbf{\hat{j}} + A_z \mathbf{\hat{k}} \) and \( \mathbf{B} = B_x \mathbf{\hat{i}} + B_y \mathbf{\hat{j}} + B_z \mathbf{\hat{k}} \), the dot product is:
\[
\mathbf{A} \cdot \mathbf{B} = A_x B_x + A_y B_y + A_z B_z
\]
This component-wise definition simplifies many electrodynamics problems, such as finding the projection of a field vector in a given direction.

### Cross Product in Component Form
The cross product in component form for the same vectors is:
\[
\mathbf{A} \times \mathbf{B} = \left( A_y B_z - A_z B_y \right) \mathbf{\hat{i}} + \left( A_z B_x - A_x B_z \right) \mathbf{\hat{j}} + \left( A_x B_y - A_y B_x \right) \mathbf{\hat{k}}
\]
This expression simplifies evaluating torques, forces, and field interactions, particularly in coordinate systems aligned with physical symmetries.

### Insight from Landau:
In continuous media, component-based vector algebra is often crucial for describing complex phenomena like anisotropic materials, where properties like permittivity and permeability vary with direction. Understanding how vectors behave in different coordinate systems is essential for analyzing the behavior of electric and magnetic fields in such media【12†source】.

## 1.1.3 Triple Products

### Scalar Triple Product
The scalar triple product of three vectors **A**, **B**, and **C** is:
\[
\mathbf{A} \cdot (\mathbf{B} \times \mathbf{C})
\]
This results in a scalar quantity that represents the volume of the parallelepiped formed by the three vectors. If the result is zero, it implies the vectors are coplanar.

### Vector Triple Product
The vector triple product is:
\[
\mathbf{A} \times (\mathbf{B} \times \mathbf{C}) = (\mathbf{A} \cdot \mathbf{C}) \mathbf{B} - (\mathbf{A} \cdot \mathbf{B}) \mathbf{C}
\]
This identity simplifies many vector calculus problems in electrodynamics, particularly when dealing with fields involving curls and vector potentials.

#### Insight from Feynman:
Feynman often uses the triple product when discussing current loops and magnetic fields, highlighting how the directionality and magnitude of fields change in complex electromagnetic systems【9†source】. The triple product is also important when analyzing **angular momentum** and rotational effects in electromagnetic fields.

## 1.1.4 Position, Displacement, and Separation Vectors

- **Position Vector**: A vector that points from the origin to a point \( P(x, y, z) \).
  \[
  \mathbf{r} = x \mathbf{\hat{i}} + y \mathbf{\hat{j}} + z \mathbf{\hat{k}}
  \]
  The position vector is a fundamental concept in defining the location of charges or field points.

- **Displacement Vector**: Describes the change in position of a particle from one point to another.
  \[
  \Delta \mathbf{r} = \mathbf{r}_2 - \mathbf{r}_1
  \]
  This is crucial in defining motion or the path integral for work done by forces.

- **Separation Vector**: The vector from one point to another in space, often used to calculate the force between two charges:
  \[
  \mathbf{r}_{12} = \mathbf{r}_2 - \mathbf{r}_1
  \]
  In electrostatics, the separation vector is used in **Coulomb’s law** to calculate the force between two charges:
  \[
  \mathbf{F} = k_e \frac{q_1 q_2}{r_{12}^2} \mathbf{\hat{r}}_{12}
  \]

### Insight from Landau:
In Landau's treatment of **macroscopic electrodynamics**, the separation vector is critical when discussing **long-range interactions** between macroscopic bodies. The relative position of different charges or bodies determines the behavior of fields, and in continuous media, understanding these vectors aids in field integration across volumes and surfaces【12†source】.

## 1.1.5 How Vectors Transform

Vectors transform according to specific rules under rotations or other coordinate transformations. For instance, under a rotation matrix **R**, the transformed vector \( \mathbf{A'} \) is:
\[
\mathbf{A'} = \mathbf{R} \mathbf{A}
\]
In electrodynamics, vector transformations ensure that physical laws hold true in all coordinate systems.

### Insight from Landau:
Landau explores vector transformations extensively when dealing with **tensor fields**, highlighting how electric and magnetic fields transform under rotations and reflections. The behavior of vectors under these transformations is essential for understanding the **Lorentz transformation** in relativistic electrodynamics【12†source】.
