---
title: RiskAdjustedLinearizations.jl
summary: A Julia package to compute risk-adjusted linearizations of dynamic economic models around the stochastic steady state

tags:
- Affine Approximation
- Perturbation Methods
- Dynamic Stochastic General Equilibrium (DSGE) Models
- Macrofinance

date: "2020-09-12T00:00:00Z"

links:
- icon: github
  icon_pack: fab
  name: GitHub Repository
  url: "https://github.com/chenwilliam77/RiskAdjustedLinearizations.jl"
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
---

# RiskAdjustedLinearizations.jl
This package implements [Lopez et al. (2018) "Risk-Adjusted Linearizations of Dynamic Equilibrium Models"](https://ideas.repec.org/p/bfr/banfra/702.html) in Julia. The [original companion code](https://github.com/fvazquezgrande/gen_affine) for the paper implements the method using MATLAB's Symbolic Math Toolbox. RiskAdjustedLinearizations.jl takes advantage of Julia's speed and flexibility so that the method can be used for solving and estimating large-scale Dynamic Stochastic General Equilibrium (DSGE) models.

Timing tests indicate that this package's speed is significantly faster than the original MATLAB code.
As examples, run the [wac_disaster.jl](https://github.com/chenwilliam77/RiskAdjustedLinearizations.jl/tree/main/examples/matlab_timing_test/wac_disaster.jl) or [rbc_cc.jl](https://github.com/chenwilliam77/RiskAdjustedLinearizations.jl/tree/main/examples/matlab_timing_test/rbc_cc.jl) scripts, which assess how long it takes to calculate a risk-adjusted linearization using the two numerical algorithms
implemented by this package and by the original authors.

## Installation

```julia
pkg> add RiskAdjustedLinearizations
```

The package is compatiable with Julia `1.x` and is tested in Linux, macOS, and Windows.
