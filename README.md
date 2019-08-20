
<!-- badges: start -->

[![Launch Rstudio
Binder](http://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/giscience-fsu/daad_summerschool_hyperspectral/master?urlpath=rstudio)
<!-- badges: end -->

Materials for the Hyperspectral session on day three of the [DAAD Summer
School](https://jupiter.geogr.uni-jena.de/summerschool/) hosted by
University of Jena in August 2019. Due to the requirement of having the
*repo2docker* config files in the repository root, a standalone
repository was created for this session. Materials of all other session
can be found [here](https://github.com/giscience-fsu/daad_summerschool).

This project was created using
[holepunch](https://karthik.github.io/holepunch) and
[repo2docker](https://github.com/jupyter/repo2docker).

  - [apt.txt](https://github.com/jupyter/repo2docker) contains the
    system dependencies
  - [runtime.txt](https://github.com/giscience-fsu/daad_summerschool_hyperspectral/blob/01a5057b9d87aaf63059cfe27703d62c024edbc3/runtime.txt)
    specifies the date of the MRAN mirror from which packages are
    installed
  - At the time of creation it was not yet possible to specify the R
    version used (<https://github.com/jupyter/repo2docker/issues/245>)
  - At the time of creation, *holepunch* was not able to declare system
    depenencies in the docker image. Therefore, the direct way via
    `repo2docker` was used.

Binder instances will shut down after 10 minutes of inactivity.

# Usage

Either click on “Launch Binder” or run locally via

``` sh
repo2docker https://github.com/giscience-fsu/daad_summerschool_hyperspectral
```

The latter requires a working installation of `docker`.
