##
# @description Base image to use Node.js in a development container
# @author      C. M. de Picciotto <d3p1@d3p1.dev> (https://d3p1.dev/)
##
FROM node:22

##
# @note Install basic development tools
##
RUN apt update && apt install -y less man-db sudo nano

##
# @note Ensure default `node` user has access to `sudo`
##
ARG USERNAME=node
RUN echo $USERNAME ALL=\(root\) NOPASSWD:ALL > /etc/sudoers.d/$USERNAME \
    && chmod 0440 /etc/sudoers.d/$USERNAME

##
# @note Set `DEVCONTAINER` environment variable to help with orientation
##
ENV DEVCONTAINER=true
