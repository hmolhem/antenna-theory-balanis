# Chapter 1 — Antennas

## 1.1 Introduction

An antenna is the transitional structure between free-space and a guiding device
(transmission line or waveguide). It converts electromagnetic energy from a guided
wave into a free-space wave (transmitting) or vice versa (receiving).

### Transmission-line equivalent circuit

The antenna is modeled as a load impedance:

$$Z_A = (R_L + R_r) + jX_A$$

- **R_r** — radiation resistance (represents actual radiation)
- **R_L** — loss resistance (conduction and dielectric losses)
- **X_A** — imaginary part associated with radiation

For maximum power transfer: conjugate matching required → $Z_g = Z_A^*$

---

## 1.2 Types of Antennas

| Type | Examples | Typical Use |
|---|---|---|
| Wire | Dipole, loop, helix | Cars, buildings, spacecraft |
| Aperture | Horn, waveguide opening | Aircraft, spacecraft |
| Microstrip (patch) | Rectangular, circular patch | Mobile devices, satellites |
| Array | Yagi-Uda, phased array | High directivity applications |
| Reflector | Parabolic, corner reflector | Deep space, radar |
| Lens | Convex-plane, concave-concave | High-frequency collimation |

---

## 1.3 Radiation Mechanism

### Key principle

$$l \frac{dI_z}{dt} = lq_l \frac{dv_z}{dt} = lq_l a_z$$

Radiation requires **time-varying current** or **acceleration/deceleration of charge**.

### Three rules

1. Charge not moving → no radiation
2. Charge moving at uniform velocity on a **straight infinite wire** → no radiation
3. Charge moving at uniform velocity on a **curved, bent, or terminated wire** → radiation
4. Charge oscillating in time-harmonic motion → radiation (even on straight wire)

### Current density relations

For volume current:
$$J_z = q_v v_z$$

For surface current (ideal conductor):
$$J_s = q_s v_z$$

For thin wire:
$$I_z = q_l v_z$$

---

## 1.4 Current Distribution on a Thin Wire Antenna

- A two-wire transmission line with very small spacing ($s \ll \lambda$) → fields cancel → no radiation
- As wires flare apart → fields no longer cancel → radiation begins
- Fully flared → dipole antenna

### Standing wave current patterns (center-fed dipole)

| Length | Pattern |
|---|---|
| $l \ll \lambda$ | Triangular approximation |
| $l = \lambda/2$ | Sinusoidal, one half-cycle per arm |
| $\lambda/2 < l < \lambda$ | Same phase throughout |
| $\lambda < l < 3\lambda/2$ | Phase reversals between half-cycles |

---

## 1.5 Historical Advancement

| Year | Event |
|---|---|
| 1873 | Maxwell publishes unified EM theory |
| 1886 | Hertz demonstrates first wireless EM system (λ = 4 m) |
| 1901 | Marconi performs first transatlantic transmission |
| 1940s | WWII launches aperture/horn/reflector antenna era |
| 1960s | Numerical methods introduced (MoM, FD, FE) |
| 1970s | Microstrip/patch antenna introduced |

---

## Key Terms

- **Radiation resistance R_r**: represents power actually radiated
- **Standing wave**: interference of incident and reflected waves
- **Conjugate matching**: $Z_g = Z_A^*$ for maximum power transfer
- **GTD/UTD**: high-frequency asymptotic method for complex structures
- **FD-TD**: solves Maxwell's equations in time domain at discrete points