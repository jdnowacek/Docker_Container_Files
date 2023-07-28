# Docker_Container_Files
# Instructions: 

# To create a docker container on a windows machine, install docker desktop or some other version of docker that includes the DOCKER ENGINE. If docker engine is not running, the commands in the dockerfile will not proceed.

# After installing docker, ensure that you have the following three files in the same folder on your machine: 

# 1. Dockerfile: the set of instructions to build your docker image. The file in its entirety is in this repo with the title: Dockerfile.txt

# 2. bdr-config: this configuration file is called by one of the commands in the dockerfile, it is also in this repo with the title bdr-config.site

# 3. An R devel tar.gz file: this file will be the most recent R-devel file from the website https://cran.r-project.org/src/base/R-4/ 
# Rename this file to R-devel.tar.gz and put it in the folder with the other two files.

# To then create your image, open a powershell window and change your directory to the folder with those three files in it and run the following command.

docker build -f Dockerfile.txt -t fedora_container .

# Yes, the dot at the end is part of the command, from there LAURA THIS IS WHERE YOUR TRICK FOR MAKING THE CONTAINER INTERACTABLE SHOULD GO.

# Your container should now be up and running, find / install R within your container and proceed to test or operate as needed.
