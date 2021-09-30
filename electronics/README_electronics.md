# Passive electronics for ion-trap based quantum technologies

## Background

Ion traps require DC and RF voltages to create the confining electric potentials that control the ion motion. The required voltages are highly dependent on the trap geometry, in particular the ion-electrode separation. For the RF, typically several hundred V at (10-100) MHz are needed. Resonant circuits are used to step up the input RF voltage, allowing to minimize the dissipation (and emission) of electric energy. For the DC, required voltages range in between a few V to a few ten V for surface traps, and up to the kV range for macroscopic traps.

Trapped ions are highly sensitive to electric field noise and supply voltages need to be filtered to reduce technical noise. The RF resonant circuit typically has a high quality factor and acts as a narrow band pass filter, reducing noise at the ions' secular frequencies. For the DC voltages, low-pass filters are typically employed. Here, one must balance the requirement of noise reduction with the need of having a sufficiently large bandwidth for the DC signals. The latter is needed for fast manipulations of the static confining potential during ion transport operations. In the design of the low-pass filters, one also needs to consider the Johnson-Nyquist noise produced in its resistive components, which adds to the electric field noise seen by a trapped ion.

## Overview of passive electronics
### Low-pass filters:
- Innsbruck, 1st order RC, 5 kHz

### RF resonators:
- [Innsbruck high-temperature superconducting resonator](passive_electronics/ibk_hts_resonator/ibk_hts_resonator.md)

## Definitions and Nomenclature

### General definitions
- _Temperature_ $`T`$. The temperature of the electric circuit.

### Low-pass filter related definitions
- _Cut-off frequency_  $`f_c`$, $`\omega_c`$ (unit: Hz, 1/s). Frequency at which a low-pass filter's response function crosses 3dB power attenuation.
- _Self-resonant frequency_  $`f_s`$, $`\omega_s`$ (unit: Hz, 1/s). Frequency above which a low-pass filter's attenuation starts to increase again, due to the parasitic inductive behaviour of the filter capacitors at high frequency.

### RF resonator related definitions
- _Inductance_ $`L`$ (unit: H). The total inductance of the resonator in an equivalent  $`RLC`$ circuit.
- _Capacitance_ $`C`$ (unit: F). The total capacitance of the resonator in an equivalent  $`RLC`$ circuit.
- _Resistance_ $`R`$ (unit: Ohm). The total resistance of the resonator in an equivalent  $`RLC`$ circuit. $`R`$ quantifies the total loss on resonance, including dielectric losses.
- _Resonance frequency_ $`f_0`$, $`\omega_0`$ (unit: Hz, 1/s). The resonance frequency of the RF step-up resonator, given by $`f_0=1/\sqrt{LC}`$, and $`\omega_0 =2\pi f_0`$.
- _Quality factor_ $`Q`$ (unit: 1). The quality factor of the RF step up resonator, defined as $`Q=2f_0/\Delta f`$, where
 $`\Delta f`$ is the measured -3 dB full-width voltage gain bandwidth of the perfectly impedance matched resonator. The quality factor can also be expressed as $`Q=\omega_0 L/R`$.
- _Voltage Gain_ $`G_V`$ (unit: 1). Step up factor of the resonator, defined as $`G_V=|U_\text{out}/U_\text{in}|`$, where $`U_\text{out}`$ is the resonator's output voltage applied to the ion trap and $`U_\text{in}`$ is the resonator's input voltage. For a perfectly impedance matched resonator, the voltage gain can be expressed as $`G_V=\sqrt{Q/(\omega_0 C R_\text{s})}`$, where $`R_\text{s}`$ is the impedance of the RF source, i.e. the cable attached to the resonator input (typically 50 $`\Omega`$).
- _Power reflection coefficient_ $`P_{ref}`$ (unit 1). The power reflection coefficient is the absolute square of the complex voltage reflection coefficient, $`P_{ref}=|V_{ref}/V_{in}|^2`$. Here, $`V_{ref}`$ and $`V_{in}`$ are the complex reflected and incoming voltage at the transition between cable and resonator, respectively.
