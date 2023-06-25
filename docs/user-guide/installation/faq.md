
# FAQ

This page contains the most common questions our users encounter.


## Update 

To install updates, download the new version of the code and container images by typing `git pull` followed by `docker-compose pull` into a terminal from your local clone of the repository. 
    

## Uninstall 
To uninstall, open a terminal in your working directory and enter your local clone of the repository (remember `ls`= list files, `cd`=change directory). Right-clicking in your working directory file explorer should give you options to open Git Bash or another terminal. If the container (or another process) is running in your terminal, you can stop it with `Ctrl+c`, or with `docker-compose down` if you see `.../noresm-land-sites-platform$`. 
    
To remove the repository, you can type `rm -r noresm-land-sites-platform` in your working directory. If it complains about permissions you may need `sudo` in front, and you can use -rf instead of -r. This might require administrator rights to your computer. NB! If you delete the whole repository like this, your existing cases and output data will also be deleted.

To delete **all** Docker containers, images, and other files, also ones in use, use the command `docker system prune -a`. NB! If you do this, you will need to download all the files again if you want to use the LSP again. It is also possible to delete everything manually in Docker desktop (check containers, images, and volumes tabs), and to delete the repository manually from your working directory.
    
Docker desktop can be uninstalled like any other program, e.g. via you pc's settings. 

## Bug or unanswered question?

Please help us by reporting errors and questions on our [issues page](https://github.com/NorESMhub/noresm-land-sites-platform/issues/new).

***************************************************

[![NorESM](img/NORESM-logo.png "the Norwegian Earth System Model")](https://www.noresm.org/)
[![EMERALD](img/Emerald_darktext_whiteBG_small.png "EMERALD project")](https://www.mn.uio.no/geo/english/research/projects/emerald/)
[![LATICE](img/UiO_LATICE_logo_black_small.png "Land-ATmosphere Interactions in Cold Environments research group")](https://www.mn.uio.no/geo/english/research/groups/latice/)

