# Setup Local Environment

## Install Git
!!! InstallGit

    === "macOS/Windows"

        Download and install [GitHub Desktop](https://desktop.github.com/)

        - Choose "Clone a Repository from the Internet..."
        - Click 'URL'

        Enter `https://github.com/AndrewBreyen/reggi-demo.git` as the URL

        - Change the directory to be YOUR-HOME-FOLDER/git/reggi-demo

    === "Linux"

        Install gh
        ```
        sudo apt install gh
        ```

        Run

        ```
        gh auth login
        ```

        and sign into GitHub




## Create `git` folder
!!! CreateFolder
    === "macOS/Linux"

        Use Finder or file explorer to create a folder, `git` in home directory

        macOS
        ```
        /Users/user/git
        ```

        Other Linux
        ```
        /home/user/git
        ```

        OR:

        In a terminal: 


        ```
        user@computer:~$ mkdir ~/git

        OR

        user@computer:~$ mkdir /home/user/git
        ``` 

    === "Windows"

        Use Windows Explorer to create a folder 


## Install `pyenv` and `python`

!!! pyenvPython
    === "macOS/Linux"

        Install Brew
        ```
        /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
        ```
        Install `pyenv` using `brew`

        ```
        brew update
        brew install pyenv
        ```

        After installing pyenv, configure your shell. 
        See: [Set up your shell environment for Pyenv: README.md](https://github.com/pyenv/pyenv#set-up-your-shell-environment-for-pyenv)


        Once configured, run:
        ```
        pyenv install 3.11.2
        ```


## Clone Repo
!!! CloneRepo
    === "Linux"

        Clone repo into /git/
        ```
        git clone git@github.com:AndrewBreyen/reggi-demo.git
        ```

        Run

        ```
        gh auth login
        ```

        and sign into GitHub

## Install Dependencies
!!! InstallDependencies

    === "macOS"

    ```
    pip install -r requirements.txt 
    ```

### Host
!!! HostMKDocs

    === "macOS"

    In a terminal, run
    ```
    cd ~/git/reggi-demo
    mkdocs serve
    ```

    Open a browser to: 
    [http://localhost:8000/](http://localhost:8000/)

