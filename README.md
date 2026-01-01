# Dark Matter Relic Density and Freeze Out (Code)

This project numerically solves the Boltzmann equation for thermal dark
matter freeze-out in the early universe. The calculation follows the
standard WIMP freeze-out framework and computes both the freeze-out
curve and the resulting relic density.

## Physical Setup

Dark matter is assumed to be a stable, massive particle that was initially
in thermal equilibrium with the Standard Model plasma. As the universe
expanded and cooled, the interaction rate dropped below the Hubble expansion
rate, causing the comoving number density to freeze out.

## Implementation

- Radiation-dominated Hubble expansion
- Maxwell–Boltzmann equilibrium number density
- Entropy density and comoving yield (Y = n/s)
- Stiff Boltzmann equation solved using `scipy.solve_ivp`
  with an implicit solver (Radau)
- Numerical identification of the freeze-out point

## Key Results
- Freeze-out at x_f ≈ 25
- Relic density Ωh² ≈ 0.1 for m = 100 GeV
