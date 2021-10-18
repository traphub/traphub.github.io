# Definitions and Nomenclature for ion traps
Back to [ion trap overview](README_ion_traps.md).

## Definitions related to the trap specifications
The trap specifications should list all key numbers of an ion trap, allowing for an assessment of the usability of a trap design for a specific application and for a quick comparison of different designs. The specifications encompass several sub categories:

### Employed materials
The materials specifications shall provide a complete list of all employed materials, including adhesive layers. Completeness of the list is a strict goal to provide full insight in vacuum-related, electric, magnetic, and thermal properties of a trap structure. For instance, magnetic materials such as nickel may cause issues in quantum optics experiments. It remains to be seen whether additional information may be necessary on the long run, such as the usage of noble gas atmospheres in the production of multilayer traps, that may subsequently result in undesired outgassing of the trap.

### Geometrical/footprint
The geometrical specifications should give an idea of the overall trap size and manufacturing quality.
- *Overall dimensions* (unit: m$$^3$$): the size, i.e. outer dimensions of the trap.
- *Feature size (min/max)* (unit: m) : the smallest and largest features of the trap. E.g., the smallest features might be electrodes or electrode leads, but also trenches between electrodes. Largest features are typically electrode outlines.
- *Manufacturing precision* (unit: m): the precision with which the features are fabricated.
- *Electrode surface roughness* (unit: m): the roughness of the electrode surface, preferably parametrized by the profile roughness parameter Ra.
- *Electrode metallization thickness* (unit: m): the thickness of metallization layer(s) in case the electrodes are formed by a coated non-conducting substrate. Place "bulk" if the electrodes are made from bulk metal.

### Interface
The interface specifications shall provide a complete list of all interfaces that need to be connected to the trap. Interfaces are grouped in categories, e.g., "electrical", "optical", "thermal", etc. For each entry, please provide the category, component description and number of channels. Typical interfaces are:
- *electrical | RF* (unit: 1, V): give the number of RF channels required for the RF confinement in the trap. Please also list the required voltage range.
- *electrical | DC low current* (unit: 1, V): give the number of low current DC channels required for the DC confinement in the trap (including shuttling operations). Please also list the required voltage range.
- *electrical | DC high current* (unit: 1, V): give the number of high current DC channels required for the generation of local B-fields (for microwave gates). Please also list the required current range.
- *optical | waveguide* (unit: 1, nm, -): give the number of integrated waveguide channels used for light routing within the trap structure. Please also list the optical wavelength and mode (single mode or multi mode).

### Optical
The optical specifications should give insight in the optical access a trap provides.
- *Optical access NA* (unit: 1): the numerical aperture (NA) of a given optical access port. Several NA values may be listed in case of multiple ports.

### Electrical
The electrical specifications should list parameters required to assess the electrical performance of the trap: RF charging currents, RF grounding properties of DC electrodes, electrical insulation and strength.
- *Capacitance RF to GND* (unit: F): the parasitic capacitance between the RF electrode and RF ground, often referred to as "trap capacitance". The trap capacitance includes the capacitance between the RF electrode and all DC electrodes in case they are intended to be grounded in the RF domain.
- *Capacitance RF to DC* (unit: F): the parasitic capacitance between the RF electrode and the specified DC electrode.
- *Capacitance DC to GND* (unit: F): the parasitic capacitance between the specified DC electrode and GND.
- *Quality factor (@ RF drive frequency)* (unit: 1): the quality factor $$Q$$ of the trap modelled as a capacitor at the RF drive frequency $$\omega_\text{rf}$$, $$Q=1/(\omega_\text{rf} C R)$$, where $$C$$ is the trap capacitance and $$R$$ is its effective resistance. In practice, a bound for the quality factor of the trap may be given by measuring the quality factor $$Q_\text{res}$$ of the resonant RF circuit used to drive the trap: $$Q = Q_\text{res}$$ if the losses in the trap dominate the losses in the resonator, and $$Q \geq Q_\text{res}$$ if losses in other resonator components (e.g. the coil) dominate.
- *Leakage current* (unit: A): the leakage current through the trap for the typical DC voltage applied to a given DC electrode. The typical DC voltage is the voltage listed under "DC confinement: maximum voltage (1 MHz axial frequency)" in the trapology-related specifications.  
- *Electric strength (breakdown voltage) DC / RF* (unit: V): the voltage, DC or RF @ RF drive frequency, at which electric breakdown occurs, i.e. the maximum applicable voltage.   

### Thermal (cryo)
The thermal specifications should state the proven operating temperature of a trap and give ratings for a vacuum bakeout.
- *Trap operation temperature* (unit: K): temperature at which the trap is operated.
- *Maximum bake-out temperature* (unit: K): maximum temperature to which the trap can be exposed for a period of several days up to a few weeks.
- *Maximum temperature ramp* (unit: K): maximum rate of temperature change to which the trap can be exposed.

### Trapology
The trapology specifications should list key numbers related to: efficiency of an electrode design to generate desired electric fields, and trap performance in terms of undesired/uncontrolled fields.
- *Ion-electrode separation* (unit: m): the distance between the ion trapping position and the nearest electrode.
- *Trapping height above surface* (unit: m): the distance between the ion trapping position and the electrode plane (for surface traps).
- *RF drive: voltage @ frequency ($$q = 0.3$$)* (unit: V @ Hz): RF voltage at the RF drive frequency which is required to reach a trap stability factor of $$q=0.3$$.  
- *DC confinement: maximum voltage (1 MHz axial frequency)* (unit: V): maximum of the absolute values of typical DC voltages applied to the individual trap electrodes for the generation of a trapping potential with 1 MHz axial frequency (in linear traps).  
- *Anharmonicity RF / DC potential (3 spatial directions)* (unit: 1): The trap anharmonicity AH in direction $$i\in\{x,y,z\}$$ is defined as $$\mathrm{AH}_i = a_4 i^2/a_2$$, where $$a_2$$ and $$a_4$$ are the quadratic and quartic coefficients, respectively, of a fourth order polynomial fit to the simulated potential.
- *Minimum characteristic distance (min over all electrodes and spatial directions)* (unit: m): the characteristic distance $$D_{i,j}$$ of a trap electrode $$j$$ relates the electric field component $$E_i^{(j)}$$ generated by that electrode at the ion position to the voltage $$V_j$$ at that electrode, $$D_{i,j}=V_j/E_i^{(j)}$$. The minimum characteristic distance is the minimum of $$D_{i,j}$$ over all electrodes $$j$$ and all components $$i$$.
- *Typical stray electric fields (3 spatial directions)* (unit: V/m): typical values for the uncontrolled stray electric field observed in a trap, e.g. the fields generated by charged dust particles or exposed dielectric surfaces. The stray field at the ion position can be identified with the electric field applied for perfect micromotion compensation, albeit with negative sign.
- *Residual micromotion modulation index (3 spatial directions)* (unit: 1): The micromotion modulation index $$\beta$$, normalized for a laser wavelength of $$\lambda=729\,$$ nm, persistent for perfect alignment of a trapped ion with the RF quadrupole. The modulation index can be directly determined from the ratio of measured Rabi rate on the micromotional sideband, $$\Omega_\text{mm}$$, and the Rabi rate on the carrier transition, $$\Omega_{car}$$. It holds $$\Omega_\text{mm}/\Omega_{car}=J_1(\beta)/J_0(\beta)$$, where $$J_i(\beta)$$ are Bessel functions of the first kind.
- *Heating rate @ secular frequency (3 spatial directions)* (unit: phonons/s): The heating rate is the rate at which an ion, initially in the motional ground state of a given secular mode, is heated to the first excited state by ambient electric field noise. Being a non-universal quantity, the heating rate needs to be specified along with motional mode frequency, the ion mass, and the ion charge. Preferably, the heating rate should be given for a secular frequency of 1 MHz and normalized to a $$^{40}\mathrm{Ca}^{+}$$ ion.

## Definitions related to the calculation of trapping potentials

### Pseudo potential and applied RF voltage
The RF confinement in a typical ion trap can to good approximation be described by a harmonic pseudo potential. The total confining potential, including the static potential generated by DC electrodes, can then be written as $$U = m \Sigma_i \omega_i^2/ 2$$, where $$m$$ is the ion mass and the sum runs over all spatial dimensions, $$i\in\{x,y,z\}$$. The secular frequency is related to the stability parameters as,

$$\omega_i = \omega_\text{rf}\sqrt{a_i + q_i^2/2}/2 \,, $$

where $$\omega_\text{rf}$$ is the RF drive frequency and $$a_i, q_i$$ are the trap stability parameters. In particular, in the limit of vanishing DC confinement, one finds
$$\omega_i \sqrt{8}/\omega_\text{rf} =  q_i \propto U_\text{rf}$$. A measurement of the secular frequencies $$\omega_i$$ for varying static confinement can typically the most precise way to determine the RF voltage $$U_\text{rf}$$ applied to the trap, if trap simulation.

### Description of trapping potentials
The electric potential $$U$$ generated by a given trap electrode (RF or DC) is best described as an expansion in terms of spherical harmonics, $$U = V \Sigma_{i,j} C_{i,j} Y_{i,j}$$, where $$V$$ is the voltage applied to the electrode (typically set to 1 V), and the $$ Y_{i,j}$$ are the spherical harmonics, up to second order,

$$Y_{1,-1} = y \,,$$

$$Y_{1,0} = z \,,$$

$$Y_{1,+1} = x \,,$$

$$Y_{2,-2} = xy \,,$$

$$Y_{2,-1} = yz \,,$$

$$Y_{2,0} = z^2-x^2-y^2 \,,$$

$$Y_{2,+1} = xz \,,$$

$$Y_{2,+2} = x^2-y^2 \,.$$

Note this definition neglects normalization prefactors. The preferred unit for the expansion coefficients is 1/mm for the 1st order coefficients $$C_{1,j}$$ and 1/mm² for the 2nd order coefficients $$C_{2,j}$$. For typical trap geometries these units lead to coefficients around 1.
