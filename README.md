# Entropic and Energetic Selectivity Analysis of Polymeric Membranes for Gas Separation

A computational framework for decomposing gas diffusion selectivity into its **energetic** (enthalpic) and **entropic** contributions in polymeric membranes, following the transition state theory formalism of Koros and co-workers.

> **Status:** 🚧 Work in progress — data and results are withheld until publication. Code and methodology are available for review.

## Background

The performance of polymer membranes for gas separation is governed by the interplay between permeability and selectivity, classically represented in Robeson plots. While the trade-off between these two properties is well established, the *underlying mechanism* driving selectivity — whether it originates from energetic barriers or entropic constraints during diffusion — is far less explored, especially for advanced materials like Polymers of Intrinsic Microporosity (PIMs) and thermally rearranged polymers.

This project provides tools to:

- Calculate activation energies of permeation (*E*<sub>p</sub>), diffusion (*E*<sub>d</sub>), and heats of sorption (*H*<sub>s</sub>) from temperature-dependent transport data via Arrhenius–van't Hoff analysis.
- Decompose diffusion selectivity into energetic and entropic components using Equation 6 from [Fuoco et al., ACS Appl. Mater. Interfaces 2018, 10, 36475–36482](https://doi.org/10.1021/acsami.8b13634).
- Visualize the results on Robeson diagrams colored by the enthalpic contribution.
- Perform multivariate statistical analysis (PCA, hierarchical clustering, correlation mapping) to identify structure–property relationships across polymer families.

## Key Dependencies

```
numpy
pandas
scipy
scikit-learn
matplotlib
openpyxl
```

## Gas Pairs and Upper Bounds

The following Robeson upper bounds are implemented:

| Gas Pair    | Upper Bounds Available       |
|-------------|------------------------------|
| CO₂/N₂     | 2008, 2019                   |
| O₂/N₂      | 1991, 2008, 2015             |
| CO₂/CH₄    | 1991, 2008, 2019, MIX 2018  |

## References

...

## License

This repository is provided for academic review purposes. Please do not redistribute data or figures without permission.

## Contact

For questions or collaboration inquiries, please open an issue.
