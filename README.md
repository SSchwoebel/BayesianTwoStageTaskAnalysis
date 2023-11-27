# BayesianTwoStageTaskAnalysis

### Description
Description and general comments go here.

### Installation instructions
 #### What you need
 The following is a little overview list of what you will need to use and to contribute. Below you find recommended tools for those in Windows or Linux
 For usage:
 1. git
 2. python, possibly with a tool for virtual environments (e.g. PIP, Anaconda)
 For contributing additionally:
 3. ssh-key for git
 4. access to the raw data (P:/10129/Experiments/BayesianTwoStageTask/raw_data)
    Raw data is only used to for preprocessing, every subsequent scipt or analysis can be run with the cleaned up data in the preprocessed_data folder.
 #### Windows:
 1. git: Github Desktop is the recommended git gui, however GitKraken also seems nice. If you want to use the command line, I recommend git-scm. Or just use Visual Studio code as an editor, it has git integration.
 2. python: Install python with Anaconda. You can also use the python_env.yml file in this folder to set up the virtual environment with the right packages. Anaconda comes with python editors as well, use jupyter for the .ipynb files and spyder for the .py files.
 3. ssh-key: Github only lets you push to a repo if you have an ssh key. Unforunately this has to be generated in the commandline. Open the command line and ...\
    run either:\
    $ ssh-keygen\
    or\
    $ ssh-keygen\
    Importantly in Windows the keygen command bugs out for the folder format, and the default file name and location it offers will not work (due to the other slash /). Type instead: C:\Users\YourName\ .ssh\id_rsa
    Go to the .ssh folder, keep the id_rsa key private, it's your private key! Open the id_rsa.pub (public key) file and copy paste the content to the SSH Key Section your Github Settings. Your Github Desktop application should see the key automatically.

 #### Linux 
 1. git: If you're using linux, you probably know git and use it in the command line.
 2. python: I recommend not using the system python, but use a virtual environment manager, to not get into version conflitcs etc. Anaconda or PIP are two alternatives and the yml file can be used to load the packages that were used in this code.
 3. ssh-key: run\
    $ ssh-keygen\
    you can leave the passphrase empty.

 #### Actual installation
 Clone the repo. This repo also contain a submodule. It points to the BalancingControl repo which contains the Bayesian behavioral agent used in this analysis. This repo keeps track of which commit itself points to. You can either just use it as is, or even set it up in a way that you can change that code from within this repo, and commit and push from here. Then you also have to tell git that the top repo should point to a new commit, by adding the folder and commiting and pushing it as any other change.
 
 When you set up the submodule, a git gui will notice that a submodule exists and ask you to set it up. Say yes. When using the commandline find more in depth instructions how to set it up in code/readme.txt