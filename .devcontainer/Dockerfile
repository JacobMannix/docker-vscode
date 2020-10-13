FROM python:3.8-slim-buster

# Options for common setup script
ARG INSTALL_ZSH="true"
ARG UPGRADE_PACKAGES="false"
ARG USERNAME=vscode
ARG USER_UID=1000
ARG USER_GID=$USER_UID

WORKDIR /python/app

COPY /.devcontainer/requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

ADD ./src/ /src
