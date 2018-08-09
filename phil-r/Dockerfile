# container with R installed
# build with: docker build <path_to_dockerfile> --tag='phil-r'
# run with: docker run -it phil-r
# after exit find container name with: docker ps -a
# start existing container: docker start -i <container_name>

FROM rocker/r-ver:3.3.1

# install Rcpp and BH
RUN R -e "install.packages(c('Rcpp', 'BH'), Ncpus=parallel::detectCores())"

# set command to run on startup
CMD ["/bin/bash"]
