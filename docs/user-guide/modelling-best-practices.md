# Model performance and best practices

While the LSP makes is easy to perform a simulation, there are many pitfalls to consider when setting up model experiments and interpreting the results. To get realistic results from simulations, three elements must be correct: model structure, model parameterization, and the external forcing data. Getting all three right is difficult even for experienced modellers, but you can get far by being curious and careful in your interpretations. Ask yourself, what can the model actually do (which processes are included in the model structure)? What do the current parameters represent (e.g. for default Plant Functional Types, mortality rates, growth allometry)? Is the forcing data realistic for my site? 

If you want to improve you model experiment, it's vital to consider your purpose. For example, do you want the output to be as similar as possible to an observed data set? If so, you might tune model parameters and adjust your input (forcing) data. The risk is that you "get the right result for the wrong reason", but that might be acceptable depending on your purpose and if you don't extrapolate. Alternatively, one might risk getting completely unrealistic model output even when all parameters and forcing data are correct. The model may lack an important process that produces a result in real life. Model calibration, validation and tuning should therefore be done with great care and according to your purpose of modelling. 

To learn more about the models and land surface modelling, check out our [external resources page](https://noresmhub.github.io/noresm-land-sites-platform/resources/). Understanding what you don't know is the first step!

## Advanced customisation

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



## Reproducibility
    
To make your simulations reproducible by others, e.g. for a thesis or scientific paper, *note down the version of the NorESM-LSP* and save these three directories that have been created under `resources/` in your working directory (e.g. C:/Users/yourusername/noresm-land-sites-platform/resources):

- the case folder, i.e. ´resources/cases/casename´
- the case input data, i.e. ´resources/data/casename´
- code modifications in overwrites, i.e. ´resources/overwrites´

You could also simply save the whole 'resources' folder (and get some redundant files).

To recreate an old simulation, the LSP might need to be reinstalled. Old case folders can of course be copied into new versions of the LSP, but if there are changes to e.g. python libraries, model code or other software we depend on, there might be errors or slight differences in the output if the case is re-run. To install a specific version, go to [GitHub](https://github.com/NorESMhub/noresm-land-sites-platform), find the correct version tag/release tag, and clone or download the code from that version. Once the correct version of the repository is in place, copy and pase in the three folders listed above. Make sure the folder structure is the same. Then, bring up the containers again with `docker-compose up` and *voilà*! 


## Reproducibility
    
To make your simulations reproducible by others, e.g. for a thesis or scientific paper, *note down the version of the NorESM-LSP* and save these three directories that have been created under `resources/` in your working directory (e.g. C:/Users/yourusername/noresm-land-sites-platform/resources):

- the case folder, i.e. ´resources/cases/casename´
- the case input data, i.e. ´resources/data/casename´
- code modifications in overwrites, i.e. ´resources/overwrites´

You could also simply save the whole 'resources' folder (and get some redundant files).

To recreate an old simulation, the LSP might need to be reinstalled. Old case folders can of course be copied into new versions of the LSP, but if there are changes to e.g. python libraries, model code or other software we depend on, there might be errors or slight differences in the output if the case is re-run. To install a specific version, go to [GitHub](https://github.com/NorESMhub/noresm-land-sites-platform), find the correct version tag/release tag, and clone or download the code from that version. Once the correct version of the repository is in place, copy and pase in the three folders listed above. Make sure the folder structure is the same. Then, bring up the containers again with `docker-compose up` and *voilà*! 


