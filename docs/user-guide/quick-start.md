# TL;DR quick start 🏃‍♀️🏃‍♂️

If you have already completed [first-time setup](https://noresmhub.github.io/noresm-land-sites-platform/user_guide/#0-prerequisites-first-time-setup) and know what you are doing, here is the extremely quick user guide. In a terminal where you have the repository: 
    
```
cd noresm-land-sites-platform
docker-compose up
```

Open the GUI: [localhost:8080](http://localhost:8080) and push buttons, and access jypyter notebooks on [localhost:8888](http://localhost:8888) and Panoply on [localhost:5800](http://localhost:5800) 🎉

***********************************************

## An overview of the LSP software

![User interfaces and simplified software architecture](img/user-interfaces-and-architecture-Page-1.jpg)

*Illustration of the user interfaces and a simplified software architecture. From your browser, you can access this user guide and our technical documentation, as well as the GUI, JupyterLab and Panoply servers once the containers are up and running (see [0. Prerequisites](https://noresmhub.github.io/noresm-land-sites-platform/user_guide/#0-prerequisites-first-time-setup) and [1. Starting the containers](https://noresmhub.github.io/noresm-land-sites-platform/user_guide/#1-start-the-container) below). Containers provide virtual computing environments where we can run the model and the software can communicate with each other. Repositories (versioned file structures) with the code for the NorESM-LSP and models are stored on GitHub. Input data is downloaded to the containers from external storage, and model output is stored locally in the user's copy of the repository. See the [Software Architecture description in the technical documentation](https://noresmhub.github.io/noresm-land-sites-platform/documentation/#software-architecture) for more details.*
