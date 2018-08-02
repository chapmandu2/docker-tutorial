# container with R installed plus a package
# build with: docker build <path_to_dockerfile> --tag='phil-r3'
# run with: docker run -it phil-r3
# after exit find container name with: docker ps -a
# start existing container: docker start -i <container_name>

FROM phil-r

# install lattice
RUN R -e "install.packages('lattice')"

# set command to run on startup
CMD ["R"]
