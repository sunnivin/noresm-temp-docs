# Advanced customisation

If you need customisation of data, model code, or case setup beyond what is possible through the graphical user interface and JupyterLab, you may access the containers or API directly. You can also [use the platform remotely, e.g. via SSH tunnelling](https://noresmhub.github.io/noresm-land-sites-platform/documentation/#running-the-noresm-lsp-remotely). 


If you have (or create) an `.env` file in the project root with `HOST_USER` set in it, use this:

```
docker-compose exec -u <host_user_value> api bash
```

Otherwise, use this:

```
docker-compose exec api bash
```

This will open a terminal in /ctsm-api. The model is in /ctsm-api/resources/model. Cases created with the api go in /ctsm-api/resources/cases, and their data in /ctsm-api/resources/data/<case-id>. The build, run, and archive folders are put inside the case folder. Shared data goes in /ctsm-api/resources/data/shared.
