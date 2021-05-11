openfaas-artifactory-headstart

# OpenFaaS Artifactory - Headstart

Based on "Artifactory and OpenFaaS – Containers Everywhere!" at https://jfrog.com/blog/artifactory-and-openfaas-containers-everywhere/

## 100 - Deploy OpenFaaS

See https://github.com/vanHeemstraSystems/openfaas-workshop-headstart

## 200 - Set your OpenFaaS prefix for new images
OpenFaaS images are stored in a Docker registry or the Docker Hub, we can set an environment variable so that your username is automatically added to new functions you create. This will save you some time over the course of the workshop.

Edit ~/.bashrc or ~/.bash_profile - create the file if it doesn't exist.

Now add the following - changing the URL as per the one you saw above (e.g. "wvanheemstra").

### Option A: Docker Hub

export OPENFAAS_PREFIX="wvanheemstra" # Populate with your Docker Hub username

### Option B: Artifactory

export OPENFAAS_PREFIX="docker-shared-images.artifactory.[YOUR COMPANY].com" # Populate with your Artifactory path
