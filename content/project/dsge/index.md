---
title: DSGE.jl
summary: A Julia framework for the solution and estimation of Dynamic Stochastic General Equilibrium (DSGE) models

tags:
- Dynamic Stochastic General Equilibrium (DSGE) models
- Bayesian Econometrics
- Simulation Methods
- State Space Models
- Time-Series Models

date: "2019-08-30T00:00:00Z"

links:
- icon: github
  icon_pack: fab
  name: GitHub Repository
  url: "https://github.com/FRBNY-DSGE/DSGE.jl"
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
---

The `DSGE.jl` package implements the New York Fed dynamic stochastic general equilibrium (DSGE) model and provides general code to estimate many user-specified DSGE models. The package is introduced in the Liberty Street Economics blog post
[The FRBNY DSGE Model Meets Julia](http://libertystreeteconomics.newyorkfed.org/2015/12/the-frbny-dsge-model-meets-julia.html).
(We previously referred to our model as the "FRBNY DSGE Model.")

This Julia-language implementation mirrors the MATLAB code included in the
Liberty Street Economics blog post
[The FRBNY DSGE Model Forecast](http://libertystreeteconomics.newyorkfed.org/2015/05/the-frbny-dsge-model-forecast-april-2015.html).

Documentation for the *code* can be accessed by clicking on the `docs|latest` button above. For documentation about the most recent *model version*, read this [pdf](https://github.com/FRBNY-DSGE/DSGE.jl/blob/main/docs/DSGE_Model_Documentation_1002.pdf).

The New York Fed DSGE team is currently extending the code to solve and estimate heterogeneous agent models. Filtering and smoothing algorithms are available in the registered package [StateSpaceRoutines.jl](https://github.com/FRBNY-DSGE/StateSpaceRoutines.jl).
An implementation of Sequential Monte Carlo (SMC) sampling, used for the estimation of DSGE models, can be found in the registered package [SMC.jl](https://github.com/FRBNY-DSGE/SMC.jl). The foundational `AbstractModel` type, from which the `AbstractDSGEModel` type derives, is defined in the registered package [ModelConstructors.jl](https://github.com/FRBNY-DSGE/ModelConstructors.jl).
