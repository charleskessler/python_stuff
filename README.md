1. Install the conda package manager
    - https://repo.anaconda.com/miniconda/Miniconda3-latest-Windows-x86_64.exe
    - this provides a command line application that will let you pull in various libraries (e.g. metpy) from the conda-forge repository
2. Once installed go to Start menu and look for `Anaconda Prompt (miniconda3)` -- this will open a command prompt window that is configured for operating with `conda` commands.
3. Create a virtual environment for your project: `conda create -n metpy_demo`
    - Type `y` to continute creating the environment
4. Once the environment is created activate it: `conda activate metpy_demo`
5. Now we can install the metpy library: `conda install -c conda-forge metpy`
    - Hit `y` to continue at the prompt
    - It will download and install the libraries `metpy` depends on 
6. One more library to install: `conda install -c conda-forge cartopy`
    - this library produces the maps
7. Once everything is installed, `cd` to the directory where you have the `isentropic_example.py` file saved
8. Run `python isentropic_example.py` and the maps should pop up after some file downloads and churning
