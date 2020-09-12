---
title: Model Constructors
summary: A Julia package to build custom model types for estimation.

tags:
- Bayesian Econometrics
- State Space Models
- Time-Series Models

date: "2019-08-11T00:00:00Z"

# Optional external URL for project (replaces project detail page).
#external_link: "https://github.com/FRBNY-DSGE/ModelConstructors.jl"

links:
- icon: github
  icon_pack: fab
  name: GitHub Repository
  url: "https://github.com/FRBNY-DSGE/ModelConstructors.jl"
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
---

This package contains the building blocks of model objects, such as `Parameter`, `Observable`, `Setting`, and `State` types. You may define any custom model, so long as it has parameters. The model object is used in both [DSGE.jl](https://github.com/FRBNY-DSGE/DSGE.jl) and [SMC.jl](https://github.com/FRBNY-DSGE/SMC.jl).

See `/docs/examples` for examples of how to construct your custom model, then use [SMC.jl](https://github.com/FRBNY-DSGE/SMC.jl) to estimate it (available for any type of model) and [DSGE.jl](https://github.com/FRBNY-DSGE/DSGE.jl) to construct forecasts, shock decompositions, impulse responses, etc. (available for DSGE models).

## Installation
`ModelConstructors.jl` is a registered Julia package in the [`General`](https://github.com/JuliaRegistries/General) registry.  To install, open your Julia REPL, type `]` (enter package manager), and run

```julia
pkg> add ModelConstructors
```

## Versioning
`ModelConstructors.jl` is currently compatible with Julia `v1.x`. To use `ModelConstructors.jl` with Julia 0.7, please use tag `v0.1.12` or lower.
