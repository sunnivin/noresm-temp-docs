# NGI template for static webpage with Mkdocs and Docker

This repository contains the NGI template for [mkdocs](https://squidfunk.github.io/mkdocs-material/).

## Symbols used in this documentation 

- Variables written in capital letters enclosed with <> are variables given by the user.

## Local development

Activate the virtual environment and run 

    ~/template-mkdocs-ngi(main)$ poetry shell
    (template-mkdocs-ngi-py3.11)~/template-mkdocs-ngi(main)$ poetry install
    (template-mkdocs-ngi-py3.11)~/template-mkdocs-ngi(main)$ mkdocs serve 

This with bring up a mkdocs server on http://localhost:8000/. 

**NB** when you work locally with `mkdocs` you might have to clean you cash memory of the browser, or try to see your new changes in *incognito mode* to be sure. 


## Build and run docker image locally

#TODO: Eva fill in a guide for depolying the webpage? 

To build and run the docker image locally run the docker compose
    
    docker compose up

This will serve the page on http://localhost:8080/

## Build docker image locally

Local build of the docker image 

    docker build -t ngi-mkdocs . 

## Deploy

To deploy a new version tag the respective commit on the main branch with the new version: "v.*.*.*".


