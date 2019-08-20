FROM rocker/binder:3.6.0
LABEL maintainer='Patrick Schratz'
USER root
COPY . ${HOME}
RUN chown -R ${NB_USER} ${HOME}
USER ${NB_USER}

RUN export DEBIAN_FRONTEND=noninteractive; apt-get -y update \
  && apt-get install -y \
 libudunits2-dev \
 libgdal-dev \
 libgeos-dev \
 ccache

RUN wget https://github.com/giscience-fsu/daad_summerschool_hyperspectral/raw/master/DESCRIPTION && R -e "options(repos = list(CRAN = 'http://mran.revolutionanalytics.com/snapshot/2019-08-20/')); devtools::install_deps()"

RUN rm DESCRIPTION.1
