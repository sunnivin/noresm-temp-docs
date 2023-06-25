
# Prerequisites (first time setup) 🌱

To use the NorESM land sites platform, you need [Git](https://git-scm.com/downloads "click the pc screen button if you are on Windows"), [Docker desktop](https://www.docker.com/products/docker-desktop), and about 15-20GB of available disk space before you can clone the [repository](https://github.com/NorESMhub/noresm-land-sites-platform "repository for the NorESM Land Sites platform") (= download the code) and start working in the containers. You may need administrator rights to your computer to install Git and Docker. If you don't want to use Git, you can try to download and unpack the repository manually instead by clicking the `code` button and `download zip`. Note that [some Mac computers may be difficult to run on](https://github.com/NorESMhub/noresm-land-sites-platform/issues/162), but otherwise any operating system that can run Docker should work. Step by step (with steps in brackets only sometimes necessary, depending on your computer):

=== "C"

    ``` c
    #include <stdio.h>

    int main(void) {
      printf("Hello world!\n");
      return 0;
    }
    ```

=== "C++"

    ``` c++
    #include <iostream>

    int main(void) {
      std::cout << "Hello world!" << std::endl;
      return 0;
    }
    ```


=== "Unix"

    1. Sed sagittis eleifend rutrum
    2. Donec vitae suscipit est
    3. Nulla tempor lobortis orci

=== "Windows"

    1. Sed sagittis eleifend rutrum
    2. Donec vitae suscipit est
    3. Nulla tempor lobortis orci



1. [Create a GitHub account](https://github.com/) (optional, but generally recommended to be able to open issues, etc.)
2. Install Git on your machine. For Windows: https://gitforwindows.org/, other: https://github.com/git-guides/install-git
3. Install [Docker desktop](https://docs.docker.com/get-docker), might require restart
4. (Install Docker Compose; should already be included in the Docker installation described above for Mac and Windows: [install docker-compose](https://docs.docker.com/compose/install) )
5. (Remarks for Windows: You may have to install WSL2 (the 'two' is important here) manually if prompted. Follow the steps described [here](https://www.omgubuntu.co.uk/how-to-install-wsl2-on-windows-10). To open the Windows Command Prompt terminal as an administrator, type `cmd` into the Windows search bar located next to the Start Symbol (lower-left corner of the screen), right-click on 'Command Prompt', and select 'Run as administrator'. Also, note that some steps in the guide are executed in the 'Command Prompt' and some are executed in the 'Windows PowerShell'; to open the latter, type 'PowerShell' into the search bar and open as administrator. If Docker complains about you not belonging to the correct 'user group' after successful installation, follow the steps described [here](https://stackoverflow.com/questions/61530874/docker-how-do-i-add-myself-to-the-docker-users-group-on-windows-10-home))
6. Open the file explorer and find a suitable folder to serve as working directory. This is where you will store the repository and installation files needed by the platform, as well as your output files (which may take up quite a bit of space!). Your working directory should be easy to find, stable, and have plenty of free space available. For instance `C:/Users/yourusername` (OneDrive, USB sticks, or your overly-cluttered desktop are not recommended 👀).
7. When you are in your chosen working directory, right-click and choose "Git Bash here" (Windows). You can also directly use `cd [path_to_working_directory]` in a terminal with Git installed. Copy and paste the following line into the terminal (note that in some terminals such as Git Bash, you need to click the right mouse button to paste from the clipboard):

```
git clone https://github.com/NorESMhub/noresm-land-sites-platform.git --config core.autocrlf=input

```

This will download (= clone) the repository (= folder structure of files with version history) to your working directory. You can now see the folder and files in your file explorer.

Once Git, Docker Desktop and the repository are in place, you don't have to do this again. 

