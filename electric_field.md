# Section 2.1: The Electric Field

The **electric field** is a fundamental concept in electrostatics. It is a vector field that represents the force per unit charge exerted on a test charge placed at any point in space by other electric charges. Electrostatics is concerned with electric fields produced by stationary charges.

## 2.1.1 Introduction

In electrostatics, we study the behavior of electric fields in the absence of moving charges. The electric field $\mathbf{E}$ at any point in space is produced by a charge distribution and can be defined in terms of the **force** $\mathbf{F}$ experienced by a small test charge $q$:

$$
\mathbf{E} = \frac{\mathbf{F}}{q}
$$

This means that the electric field is the force per unit charge at a given point. The electric field is a vector, meaning it has both magnitude and direction.

#### Conceptual Understanding:
The electric field at any point is determined by the configuration of charges in space. It obeys the **principle of superposition**, which means the total field is the sum of the fields due to each individual charge.

<br>

## 2.1.2 Coulomb’s Law

**Coulomb's law** describes the electrostatic interaction between two point charges. The force $\mathbf{F}$ between two charges $q_1$ and $q_2$ separated by a distance $r$ is:

$$
\mathbf{F} = \frac{1}{4 \pi \epsilon_0} \frac{q_1 q_2}{r^2} \hat{\mathbf{r}}
$$

Where:
- $\epsilon_0$ is the **permittivity of free space** ($\epsilon_0 = 8.854 \times 10^{-12} \, \text{C}^2 / \text{N} \cdot \text{m}^2$).
- $r$ is the distance between the two charges.
- $\hat{\mathbf{r}}$ is the unit vector pointing from one charge to the other.

#### Field Produced by a Point Charge:
The electric field $\mathbf{E}$ produced by a point charge $q$ located at $\mathbf{r}'$ is given by:

$$
\mathbf{E}(\mathbf{r}) = \frac{1}{4 \pi \epsilon_0} \frac{q}{|\mathbf{r} - \mathbf{r}'|^2} \hat{\mathbf{r}}_{r' \to r}
$$

Where $\mathbf{r}$ is the position where the field is measured, and $\hat{\mathbf{r}}_{r' \to r}$ is the unit vector pointing from the charge at $\mathbf{r}'$ to the field point $\mathbf{r}$.

#### Applications:
- **Coulomb's law** forms the basis for calculating the electric field in electrostatics. It is the starting point for analyzing fields due to discrete charges and understanding the behavior of electric fields in free space.

<br>

## 2.1.3 The Electric Field

The **electric field** $\mathbf{E}$ is a vector field produced by electric charges. It describes the force per unit charge experienced by a small positive test charge placed in the field. The direction of the electric field is the direction of the force on a positive charge.

For a point charge $q$, the electric field at a distance $r$ is:

$$
\mathbf{E} = \frac{1}{4 \pi \epsilon_0} \frac{q}{r^2} \hat{\mathbf{r}}
$$

#### Field Lines:
Electric field lines are used to visualize the electric field. These lines:
- Emanate from positive charges and terminate on negative charges.
- Are tangent to the electric field vector at any point.
- Never cross each other.

The **density of field lines** represents the strength of the electric field: where the lines are close together, the field is stronger.

#### Principle of Superposition:
The electric field obeys the **principle of superposition**. For a system of charges $q_1, q_2, \dots, q_N$, the total electric field at a point $\mathbf{r}$ is the vector sum of the fields produced by each individual charge:

$$
\mathbf{E}(\mathbf{r}) = \sum_{i=1}^{N} \mathbf{E}_i(\mathbf{r})
$$

This principle allows us to calculate the total field for systems of multiple charges by simply adding the contributions from each charge.

<br>

## 2.1.4 Continuous Charge Distributions

In many physical systems, charge is distributed continuously, rather than being confined to discrete points. The electric field produced by a **continuous charge distribution** is obtained by integrating Coulomb’s law over the volume of the charge distribution.

For a charge distribution with **volume charge density** $\rho(\mathbf{r})$, the electric field at a point $\mathbf{r}$ is:

<p assign="center">
$$\mathbf{E}(\mathbf{r}) = \frac{1}{4 \pi \epsilon_0} \int \frac{\rho(\mathbf{r}')}{|\mathbf{r} - \mathbf{r}'|^2} \hat{\mathbf{r}}_{r' \to r} \, d^3r'$$
</p>

Where:
- $\rho(\mathbf{r}')$ is the charge density at position $\mathbf{r}'$.
- The integral is carried out over the entire volume of the charge distribution.

#### Surface and Line Charge Distributions:
- For a **surface charge density** $\sigma(\mathbf{r})$ distributed over a surface, the electric field is:

  <p assign="center">
  $$\mathbf{E}(\mathbf{r}) = \frac{1}{4 \pi \epsilon_0} \int_S \frac{\sigma(\mathbf{r}')}{|\mathbf{r} - \mathbf{r}'|^2} \hat{\mathbf{r}}_{r' \to r} \, dA'$$
  </p>
  
- For a **line charge density** $\lambda(\mathbf{r})$ distributed along a line, the electric field is:

  <p assign="center">
  $$\mathbf{E}(\mathbf{r}) = \frac{1}{4 \pi \epsilon_0} \int_L \frac{\lambda(\mathbf{r}')}{|\mathbf{r} - \mathbf{r}'|^2} \hat{\mathbf{r}}_{r' \to r} \, dl'$$
  </p>
  
#### Example: Uniformly Charged Rod
Consider a uniformly charged rod of length $L$ and total charge $Q$. The charge density is $\lambda = Q/L$. The electric field at a point $\mathbf{r}$ due to the rod can be calculated by integrating Coulomb’s law along the length of the rod.

---

## **Additional Sections (from Landau, Feynman, and earlier editions of Griffiths)**

### 2.1.5 Electrostatic Fields in Continuous Media (Landau)

In **Landau’s Electrodynamics of Continuous Media**, the behavior of electric fields in **continuous media** is explored. When charges are placed in dielectric materials, the **electric displacement field** $\mathbf{D}$ is introduced to account for the effects of the material's polarization. The displacement field relates to the electric field $\mathbf{E}$ and the **polarization** $\mathbf{P}$ of the medium as follows:

<p assign="center">
$$\mathbf{D} = \epsilon_0 \mathbf{E} + \mathbf{P}$$
</p>

#### Applications:
In dielectrics, the field due to **bound charges** (from polarization) and **free charges** are treated separately. Landau’s approach extends the analysis of electrostatic fields to media with complex internal structures, such as anisotropic dielectrics.

<br>

### 2.1.6 Feynman’s Intuition on Electric Fields

In the **Feynman Lectures**, Feynman emphasizes the conceptual understanding of electric fields by discussing how **test charges** behave in response to electric fields. He illustrates key concepts such as:

- **Visualizing Field Lines**: Feynman explains how field lines are an excellent way to visualize the influence of charges. He points out that field lines behave like **tensioned strings** between charges, which helps in understanding the interaction between charges.
  
- **Energy of the Field**: Feynman introduces the idea that the **energy** in an electrostatic system is stored in the field itself, rather than in the individual charges. This concept is later formalized when discussing the energy density of the electric field.

<br>

### 2.1.7 Electric Fields from Spherical Charge Distributions (Griffiths, earlier editions)

In earlier editions of **Griffiths**, there is a detailed discussion on **spherical charge distributions**, particularly the electric field inside and outside a uniformly charged sphere. Using **Gauss’s law**, we can show:

- **Outside the Sphere**: The electric field behaves as if all the charge were concentrated at the center.

  $$\mathbf{E} = \frac{1}{4 \pi \epsilon_0} \frac{Q}{r^2} \hat{\mathbf{r}} \quad \text{for} \, r > R$$
  
- **Inside the Sphere**: The field increases linearly with distance from the center.

  $$\mathbf{E} = \frac{1}{4 \pi \epsilon_0} \frac{Qr}{R^3} \hat{\mathbf{r}} \quad \text{for} \, r < R$$
  
This approach is important for analyzing charge distributions with spherical symmetry, such as in **conducting spheres** and **charged shells**.

---
