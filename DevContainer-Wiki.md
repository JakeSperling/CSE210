Welcome to the DevContainer wiki! 
The development container is provided to help you set up the development quickly and easily. 
This wiki offers detailed instructions about how to use the devcontainer. 

## Accept Homework Assignments via GitHub Classroom

On the Canvas assignment page, there is a GitHub Classroom link.
After clicking this link, GitHub Classroom will guide you to accept the homework, and create a
GitHub repository containing all the files needed for the homework.

The instructions below assume you have accepted the homework and created the repository.

## Using the devcontainer

Generally, this devcontainer is designed to work with VSCode IDE. 
And there are two approaches to use it: 
either through GitHub Codespace or a local VSCode installation.

### GitHub Codespace

GitHub Codespaces is an online IDE derived from VSCode. 
You can access it through a web browser, so you don't need to install additional 
software on your computer.
But, Internet access is required.
This approach is not recommended 
if you are likely to work on your homework in an environment 
without stable Internet access.

1. Open your repository on GitHub
2. Click on the `< > Code` button

   <img width="500" src="https://github.com/UCSC-CSE-210A/devcontainer/assets/12905747/d467630c-88da-418d-b2a4-f39799f30031">

3. Click `Create codespace on main`
4. A new window/tab will be opened, and GitHub is creating the development environment using the devcontainer

   <img width="600" src="https://github.com/UCSC-CSE-210A/devcontainer/assets/12905747/c5e1ce9c-ba03-4c1c-8e2d-ea7e37e2570e">

5. Once the setup is completed, a VSCode IDE will be shown, and ready for use.

### Local VSCode

This approach requires you to install a few softwares on your local computer, 
but once it is set up, no Internet connection is required.

1. Install VSCode
   (It's very likely that you have already installed VSCode for your regular use 
    or for other courses; but if not, please follow the page at: 
    https://code.visualstudio.com)
2. Install Docker: https://www.docker.com/get-started/
3. Clone your repository to your local computer
4. Make sure Docker is up and running in the background
5. In VSCode, open the folder containing your repository
6. Reopen the folder in Dev Container, and there are two approaches
   - Right after you open the folder in VSCode, a notification will pop up 
     in the bottom right corner asking if you want to reopen the folder 
     in Dev Container;
     click `Reopen in Container`

     <img width="450" src="https://github.com/UCSC-CSE-210A/devcontainer/assets/12905747/9e33165c-260e-499f-94f6-9217d802090e">

   - If you missed that notification, open the command palette in VSCode (https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette), then search and click "Dev Containers: Reopen in Container"

     <img width="550" src="https://github.com/UCSC-CSE-210A/devcontainer/assets/12905747/5fb953f2-87e0-4f5e-af3d-b910189a843d">

7. A new VSCode window will be opened, and please wait for it to complete the setup process (usually this only takes 1~2 minutes)

## Some useful Coq related commands in VSCode

- open the command palette in VSCode (https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette)
- search for "Coq: "
- These four commands might be often used in this course:

  <img width="600" src="https://github.com/UCSC-CSE-210A/devcontainer/assets/12905747/7987ae55-f4d5-4eb7-bfb7-da03a63f1107">

  - **Open proof view**: this command will open a tab on the side showing the details of the current proof step
  - **Interpret to Point**: Interpret/run the code from the beginning to the location where the cursor is
    - Note that the proof view on the side will show the details of the proof at this point
  - **Step Forward**/**Step Backward**: Move 1 step further (or roll back 1 step)
    - Note that the proof view on the side will show the details of the proof at this point
- On the right-hand side of the command palette, the hotkey of the corresponding command will be shown, 
  so you can execute the command without opening the command palette every time

## Setup development environment without using the devcontainer

You may also follow the instructions here: https://coq.inria.fr/opam-using.html to install Coq manually on your local machine.
And please make sure that you are going to install Coq version 8.16.0 or 8.16.1
