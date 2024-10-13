# Section 2.3: Electric Potential

The **electric potential** is a scalar quantity that simplifies the analysis of electrostatic fields. Instead of dealing with the vector field $\mathbf{E}$ directly, we can describe the system in terms of a potential function $\phi$, from which the electric field is derived. The electric potential is especially useful in systems with high symmetry, and in solving boundary-value problems.

---

## 2.3.1 Introduction to Potential

The **electric field** $\mathbf{E}$ is related to the electric potential $\phi$ through the following relationship:

$$\mathbf{E} = -\nabla \phi$$

The electric potential is a scalar field whose gradient gives the electric field. This relationship holds for **electrostatic fields**, which are conservative, meaning that the work done by the electric field on a charge moving between two points is independent of the path taken.

### Potential Difference

The **potential difference** $V_{12}$ between two points 1 and 2 is defined as the line integral of the electric field:

$$V_{12} = \phi(\mathbf{r}_1) - \phi(\mathbf{r}_2) = -\int_{\mathbf{r}_1}^{\mathbf{r}_2} \mathbf{E} \cdot d\mathbf{l}$$

In practice, we often define the potential relative to some reference point, often taken at infinity where the potential is zero.

#### Example:
For a point charge $q$, the electric potential at a distance $r$ from the charge is:

$$\phi(r) = \frac{1}{4 \pi \epsilon_0} \frac{q}{r}$$

---

## 2.3.2 Comments on Potential

### 1. The Potential is Not Unique

The electric potential $\phi$ is not unique because we can always add a constant to the potential without changing the electric field. This is because the gradient of a constant is zero, and hence does not affect the relationship $\mathbf{E} = -\nabla \phi$.

### 2. Conservative Nature of Electrostatic Fields

The fact that electrostatic fields are conservative implies that the **line integral** of the electric field around any closed loop is zero:

$$\oint \mathbf{E} \cdot d\mathbf{l} = 0$$

This result follows from the fact that $\mathbf{E}$ is the gradient of a scalar function $\phi$. As a consequence, the potential difference between two points depends only on the endpoints, not on the path taken between them.

---

## 2.3.3 Poisson’s Equation and Laplace’s Equation

The relationship between the electric field and the potential can be expressed in a more compact form using the **divergence of the electric field**. From **Gauss’s law**, we have:

$$
\nabla \cdot \mathbf{E} = \frac{\rho}{\epsilon_0}
$$

Substituting $\mathbf{E} = -\nabla \phi$, this becomes **Poisson’s equation**:

$$
\nabla^2 \phi = -\frac{\rho}{\epsilon_0}
$$

Where:
- $\rho$ is the **charge density**.
- $\epsilon_0$ is the **permittivity of free space**.

In regions where there is no charge ($\rho = 0$), Poisson’s equation reduces to **Laplace’s equation**:

$$
\nabla^2 \phi = 0
$$

#### Physical Meaning:
- **Poisson’s equation** describes how the electric potential is related to the charge distribution in space.
- **Laplace’s equation** applies in regions of space free from charge and is widely used in solving boundary-value problems.

---

## 2.3.4 The Potential of a Localized Charge Distribution

For a **localized charge distribution** with charge density $\rho(\mathbf{r})$, the potential at a point $\mathbf{r}$ is given by:

$$
\phi(\mathbf{r}) = \frac{1}{4 \pi \epsilon_0} \int \frac{\rho(\mathbf{r}')}{|\mathbf{r} - \mathbf{r}'|} \, d^3r'
$$

This integral sums the contributions to the potential from each infinitesimal charge element $d^3r'$ of the charge distribution. For point charges, this expression reduces to the familiar formula for the potential of a point charge.

#### Example: Uniformly Charged Sphere
For a uniformly charged sphere with total charge $Q$ and radius $R$:
- **Outside the sphere** ($r \geq R$):
  
  $$ 
  \phi(r) = \frac{1}{4 \pi \epsilon_0} \frac{Q}{r}
  $$

- **Inside the sphere** ($r < R$):

  $$ 
  \phi(r) = \frac{1}{4 \pi \epsilon_0} \frac{Q}{2R} \left(3 - \frac{r^2}{R^2} \right)
  $$

This shows how the potential behaves differently inside and outside a uniformly charged spherical shell or solid sphere.

---

## 2.3.5 Boundary Conditions

When solving Poisson’s or Laplace’s equations, boundary conditions must be specified to obtain a unique solution. There are two types of boundary conditions commonly encountered in electrostatics:

### 1. Dirichlet Boundary Condition:
The potential $\phi$ is specified on the boundary of the region of interest.

$$
\phi_{\text{boundary}} = \phi_0
$$

### 2. Neumann Boundary Condition:
The normal component of the electric field (or equivalently, the derivative of the potential) is specified on the boundary.

$$
\frac{\partial \phi}{\partial n} \Big|_{\text{boundary}} = \sigma
$$

Where $\sigma$ is related to the surface charge density on the boundary.

#### Physical Meaning:
- In the **Dirichlet condition**, we know the potential values on the boundary, which is common in problems involving conductors where the potential is constant on the surface.
- In the **Neumann condition**, we specify the electric field normal to the boundary, often used in systems where we know the surface charge distribution.

---

## **Additional Sections (from Landau, Feynman, and earlier editions of Griffiths)**

### 2.3.6 The Potential in Continuous Media (Landau)

In **Landau’s Electrodynamics of Continuous Media**, the behavior of the electric potential in **polarizable materials** is discussed. When dielectrics are present, the potential is influenced by the **polarization** of the medium. The potential satisfies a modified Poisson equation:

$$
\nabla^2 \phi = -\frac{\rho_{\text{free}}}{\epsilon_0} - \frac{\nabla \cdot \mathbf{P}}{\epsilon_0}
$$

Where:
- $\rho_{\text{free}}$ is the free charge density.
- $\mathbf{P}$ is the **polarization** of the material.

#### Polarization Charges:
The term $\nabla \cdot \mathbf{P}$ represents the **bound charges** due to polarization. The presence of polarization modifies the potential in dielectrics, creating complex interactions between free and bound charges.

<br>

### 2.3.7 Feynman on Electric Potential and Energy

In the **Feynman Lectures**, Feynman provides an intuitive discussion of the relationship between **electric potential** and **energy**. He emphasizes that the **potential energy** stored in an electrostatic system is related to the configuration of charges and the electric potential:

$$
U = \frac{1}{2} \int \rho(\mathbf{r}) \phi(\mathbf{r}) \, d^3r
$$

This formula shows that the potential energy is a product of the charge density and the potential at each point in space. Feynman’s approach highlights how energy is stored in the electric field itself, rather than in the charges.

<br>

### 2.3.8 Multipole Expansion of the Potential (Griffiths, earlier editions)

In earlier editions of **Griffiths**, the **multipole expansion** of the potential is discussed for **localized charge distributions**. The potential at a point far away from a localized charge distribution can be expanded in terms of **multipoles**:

$$
\phi(\mathbf{r}) = \frac{1}{4 \pi \epsilon_0} \left( \frac{q}{r} + \frac{\mathbf{p} \cdot \hat{\mathbf{r}}}{r^2} + \frac{1}{2} \frac{Q_{ij} \hat{r}_i \hat{r}_j}{r^3} + \dots \right)
$$

Where:
- $q$ is the **monopole moment** (total charge).
- $\mathbf{p}$ is the **dipole moment**.
- $Q_{ij}$ is the **quadrupole moment**.

This expansion is particularly useful for calculating the potential of charge distributions when the observation point is far from the charges.

---

### Conclusion:

**Section 2.3: Electric Potential** introduces the concept of electric potential and how it relates to the electric field. **Poisson’s and Laplace’s equations** are central to electrostatics and are used to solve for the potential in regions with and without charge. The additional sections from **Landau** and **Feynman** provide a deeper understanding of the potential in continuous media and its relationship to energy, while earlier editions of Griffiths discuss **multipole expansions** for complex charge distributions.
