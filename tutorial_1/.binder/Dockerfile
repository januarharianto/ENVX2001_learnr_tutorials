FROM shiny
LABEL maintainer='Januar Harianto'
USER root
COPY . ${HOME}
RUN chown -R ${NB_USER} ${HOME}
USER ${NB_USER}



RUN wget https://github.com/januarharianto/ENVX2001_learnr_tutorials/raw/main/DESCRIPTION && R -e "options(repos = list(CRAN = 'http://mran.revolutionanalytics.com/snapshot/2022-02-20/')); devtools::install_deps()"

RUN rm DESCRIPTION.1; exit 0
