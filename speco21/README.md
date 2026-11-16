# Distance decay of community similarity in river networks

**Slides:** [fsdias.github.io/presentations/speco21](https://fsdias.github.io/presentations/speco21/)

Talk given at the **20.º Encontro Nacional de Ecologia** (the national ecology meeting of the Portuguese Ecological Society, SPECO), November 2021. The slides are in Portuguese.

**Title:** Analysing the distance decay of community similarity in river networks using Bayesian methods

**Authors:** Filipe S. Dias, Michael Betancourt, Patrícia María Rodríguez-González & Luís Borda-de-Água

## Summary

The talk asks whether neutral or niche-based processes drive the decline in similarity between riparian plant communities as the distance between them increases.

- **Data:** 338 riparian vegetation plots in 11 river basins in Portugal, sampled in 2003–2006. Community similarity is the Sørensen index between every pair of plots in the same basin.
- **Neutral covariates:** distance along the river network and connection through water flow.
- **Niche covariates:** difference in precipitation and difference in Strahler stream order.
- **Model:** a Bayesian model of pairwise similarity, fitted in Stan.
- **Main result:** both neutral and environmental factors are associated with the decay in similarity, which agrees with the continuum hypothesis.

## Publication

The study is published in *Scientific Reports*:

> Dias, F. S., Betancourt, M., Rodríguez-González, P. M. & Borda-de-Água, L. (2021). Analysing the distance decay of community similarity in river networks using Bayesian methods. *Scientific Reports*, 11, 21660. [https://doi.org/10.1038/s41598-021-01149-x](https://doi.org/10.1038/s41598-021-01149-x)

The slides point to the earlier preprint ([doi:10.32942/osf.io/sn5jr](https://doi.org/10.32942/osf.io/sn5jr)). Please cite the published article.

## Files

| Path | Content |
|---|---|
| `index.html` | The slides |
| `img/` | Figures and logos used in the slides |
| everything else | The reveal.js framework (`dist/`, `css/`, `js/`, `plugin/`) and its examples and tests |
