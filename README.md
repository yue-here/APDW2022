# APDW2022

### Python for synchrotron tutorial
### Overview
Python is the most popular language for scientific programming. By learning how to manipulate diffraction data with python, we take can advantage of the huge library of open source data analysis software. 

Jupyter is a framework for using "notebooks", a type of file where active python code and annotations live side-by-side. Using jupyter notebooks, we can make our data processing more transparent and shareable.

Our aims for this session:
* Understand the best way to set up python and jupyter
* Read common diffraction file formats into python data structures 
* Perform some common operations:
  * Plot a diffraction pattern
  * Plot an in situ diffracion heatmap
  * Save an animation
  * Perform some common operations on the data

### Getting the tutorial files
We will use github to download the tutorial files. Open a terminal window and navigate to the folder where you want to download the files. Then run `git clone https://github.com/yue-here/APDW2022`.

Alternatively, you can download the repository manually from the website and extract it to a folder of your choosing, from where you will launch your terminal in the next step. (In general, we recommend you use a directory with no spaces, as they can cause troubles in some cases.)

### Setting up python
Python is a programming language. Packages are pieces of code people have written that you can then install and use.

Conda is a 'environment and package manager'. Environments are used to separate different installations of python (for example if at different times you need two python packages that conflict with each other).

Anaconda is a popular distribution of conda which installs python plus a lot of the most commonly used packages.

If you want to learn more - read [this](https://geohackweek.github.io/Introductory/01-conda-tutorial/) or [this](https://problemsolvingwithpython.com/01-Orientation/01.02-The-Anaconda-Distribution-of-Python/).

Here, we will install Anaconda - get it directly from https://www.anaconda.com/.

While Anaconda's base environment is fine for our purposes, we will create a new environment for this tutorial. Open a terminal (anaconda prompt in Windows, or you can do it through the anaconda navigator 'environments' tab) in the base tutorial folder and type:
`$ conda env create -f APDW.yml`

This will recreate an environment previously tested for this tutorial from the file `APDW.yml`. To start working in the environment, type:
`$ conda activate APDW2022`

You'll also need to install the ffdmpeg package in order to create an animation during the tutorial. Note that this will only install inside the APDW2022 environment.
`$conda install ffmpeg`

### Starting jupyter
Once anaconda is installed, we start jupyter through the anaconda navigator. We will use jupyter lab - start it by clicking on the jupyter lab icon or running `jupyter lab` in a terminal.

Now, open `APDW2022_python.ipynb` in jupyter lab. The tutorial continues in this notebook.
