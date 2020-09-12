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

[![GitHub release](https://img.shields.io/github/release/chenwilliam77/RiskAdjustedLinearizations.jl.svg)](https://github.com/chenwilliam77/RiskAdjustedLinearizations.jl/releases/latest)
[![](https://img.shields.io/badge/docs-stable-3f51b5.svg)](https://chenwilliam77.github.io/RiskAdjustedLinearizations.jl/dev)
[![](https://img.shields.io/badge/docs-latest-3f51b5.svg)](https://chenwilliam77.github.io/RiskAdjustedLinearizations.jl/dev)
[![Master Build Status](https://travis-ci.com/chenwilliam77/RiskAdjustedLinearizations.jl.svg?branch=master)](https://travis-ci.com/github/chenwilliam77/RiskAdjustedLinearizations.jl)
[![Coverage Status](https://coveralls.io/repos/github/chenwilliam77/RiskAdjustedLinearizations.jl/badge.svg?branch=master)](https://coveralls.io/github/chenwilliam77/RiskAdjustedLinearizations.jl?branch=master)

This package implements [Lopez et al. (2018) "Risk-Adjusted Linearizations of Dynamic Equilibrium Models"](https://ideas.repec.org/p/bfr/banfra/702.html) in Julia. The [original companion code](https://github.com/fvazquezgrande/gen_affine) for the paper implements the method using MATLAB's Symbolic Math Toolbox. RiskAdjustedLinearizations.jl takes advantage of Julia's speed and and flexibility so that the method can be used for solving and estimating large-scale Dynamic Stochatic General Equilibrium (DSGE) models. Initial timing tests (see [examples/wachter_disaster_risk/example_wachter.jl](https://github.com/chenwilliam77/RiskAdjustedLinearizations/tree/master/examples/wachter_disaster_risk/example_wachter.jl).) indicate that this package is two orders of magnitude faster than the MATLAB implementation provided by Lopez et al. (2018).



## Installation

```julia
pkg> add RiskAdjustedLinearizations
```

The package is compatiable with Julia `1.x` and is tested in Linux, macOS, and Windows.
