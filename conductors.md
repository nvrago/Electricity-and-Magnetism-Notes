# Section 2.5: Conductors

Conductors are materials where electric charge can move freely. In electrostatics, conductors exhibit unique properties, as charges rearrange themselves until electrostatic equilibrium is reached. This section covers the fundamental properties of conductors, the behavior of induced charges, and applications such as capacitors.

---

## 2.5.1 Basic Properties

### 1. Electric Field Inside a Conductor
In electrostatic equilibrium, the electric field **inside a conductor** is always zero. If there were a nonzero electric field, free charges in the conductor would move in response to the force exerted by the field, contradicting the assumption of equilibrium.

$$
\mathbf{E}_{\text{inside}} = 0
$$

### 2. Electric Potential Inside a Conductor
Since the electric field is zero inside the conductor, the **electric potential** is **constant** throughout the conductor. The potential at any point on or inside the conductor is the same:

$$
\phi_{\text{inside}} = \text{constant}
$$

### 3. Charge on the Surface
Any excess charge placed on a conductor in electrostatic equilibrium resides entirely on the **surface** of the conductor. This is because charges repel each other, and the only stable configuration is when they spread out on the surface.

#### Example:
For a spherical conductor, all excess charge moves to the outer surface. Inside the conductor, the electric field is zero.

---

## 2.5.2 Induced Charges

When a conductor is placed in an external electric field, **induced charges** will redistribute themselves on the surface of the conductor to cancel the external field inside the conductor. This redistribution ensures that the electric field inside remains zero.

### Example: Conductor in a Uniform Electric Field
Consider a spherical conductor placed in a uniform external electric field $\mathbf{E}_0$. Charges rearrange on the surface of the sphere such that the resulting electric field inside the sphere is zero. The field outside the sphere is distorted due to the induced surface charges.

---

## 2.5.3 Surface Charge and the Force on a Conductor

### Surface Charge Distribution

The **surface charge density** $\sigma$ on a conductor depends on the local electric field near the surface. The surface charge density is related to the electric field just outside the surface of the conductor by:

$$
\sigma = \epsilon_0 \mathbf{E}_{\text{outside}} \cdot \hat{\mathbf{n}}
$$

Where:
- $\sigma$ is the **surface charge density**.
- $\mathbf{E}_{\text{outside}}$ is the electric field just outside the conductor.
- $\hat{\mathbf{n}}$ is the unit vector normal to the surface.

This expression shows that the stronger the electric field near the surface, the greater the surface charge density.

### Force on a Conductor

The electric field exerts a force on the surface charges of a conductor. The **force per unit area** on the conductor’s surface is given by:

$$
\mathbf{f} = \sigma \mathbf{E}_{\text{outside}}
$$

Where $\mathbf{f}$ is the **force per unit area** on the surface of the conductor.

#### Example: Force on a Parallel Plate Capacitor
In a parallel plate capacitor, the force on each plate due to the surface charges is proportional to the electric field between the plates and the surface charge density.

---

## 2.5.4 Capacitors

A **capacitor** is a device used to store electric charge and energy. It consists of two conductors (called **plates**) separated by an insulating material (called a **dielectric** or **vacuum**). The capacitance $C$ of a capacitor is defined as the ratio of the charge $Q$ on one conductor to the potential difference $V$ between the two conductors:

$$
C = \frac{Q}{V}
$$

### Parallel Plate Capacitor

For a **parallel plate capacitor**, with plate area $A$ and separation distance $d$, the capacitance is:

$$
C = \frac{\epsilon_0 A}{d}
$$

Where:
- $\epsilon_0$ is the permittivity of free space.
- $A$ is the area of each plate.
- $d$ is the separation between the plates.

### Energy Stored in a Capacitor

The energy $U$ stored in a capacitor is given by:

$$
U = \frac{1}{2} C V^2
$$

This shows that the energy stored in a capacitor is proportional to both the capacitance and the square of the potential difference.

---

## **Additional Sections (from Landau, Feynman, and earlier editions of Griffiths)**

### 2.5.5 Conductors in Continuous Media (Landau)

In **Landau’s Electrodynamics of Continuous Media**, conductors are examined in the context of **polarization** and **dielectric materials**. When a conductor is placed in a dielectric medium, the surrounding dielectric modifies the behavior of the induced charges and the electric field near the conductor.

- The **electric displacement field** $\mathbf{D}$ plays an important role in describing the interaction between the conductor and the surrounding dielectric:

  $$
  \nabla \cdot \mathbf{D} = \rho_{\text{free}}
  $$

Where $\rho_{\text{free}}$ represents the free charges on the surface of the conductor.

---

### 2.5.6 Feynman on Conductors and Capacitors

In the **Feynman Lectures**, Feynman provides insights into the behavior of conductors and capacitors, emphasizing practical applications. Feynman discusses how energy is stored in capacitors, using the example of a **parallel plate capacitor** to demonstrate the concepts of **capacitance** and **energy storage**.

#### Example: Energy in a Capacitor
Feynman emphasizes that the energy stored in a capacitor is in the **electric field** between the plates, with the energy density given by:

$$
u = \frac{\epsilon_0}{2} \mathbf{E}^2
$$

This field-based approach aligns with the idea that energy in electrostatic systems is stored in the field itself.

---

### Conclusion:

**Section 2.5: Conductors** explores the fundamental properties of conductors in electrostatics, such as the absence of an electric field inside and the distribution of surface charge. The section also covers the concept of induced charges, the force on a conductor, and capacitors, which are essential for storing electric energy. The additional insights from **Landau** and **Feynman** provide further understanding of conductors in continuous media and energy storage in capacitors.
