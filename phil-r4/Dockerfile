# container with R installed plus a package with system deps
# build with: docker build <path_to_dockerfile> --tag='phil-r3'
# run with: docker run -it phil-r
# after exit find container name with: docker ps -a
# start existing container: docker start -i <container_name>

FROM phil-r

# install linux system deps
RUN apt-get update && \
	apt-get install libxml2-dev

# install xlm2
RUN R -e "install.packages('xml2')"

# set command to run on startup
CMD ["R"]
