# MetaOps

[Original repository on GitHub](https://github.com/Hvass-Labs/MetaOps)

Original author is [Magnus Erik Hvass Pedersen](http://www.hvass-labs.org)


## Introduction

This is a small collection of research papers on automatic tuning of the parameters
of a heuristic optimizer such as
[Genetic Algorithm](https://en.wikipedia.org/wiki/Genetic_algorithm),
[Particle Swarm Optimization](https://en.wikipedia.org/wiki/Particle_swarm_optimization),
and [Differential Evolution](https://en.wikipedia.org/wiki/Differential_evolution).
The parameter tuning is done by another overlaying optimizer and this is often called
[Meta-Optimization](https://en.wikipedia.org/wiki/Meta-optimization)
or [Hyper-Parameter Optimization](https://en.wikipedia.org/wiki/Hyperparameter_optimization).


## Papers

1. Bayesian Meta-Optimization ([Notebook](https://github.com/Hvass-Labs/MetaOps/blob/master/01_Bayesian_Meta-Optimization.ipynb)) ([Google Colab](https://colab.research.google.com/github/Hvass-Labs/MetaOps/blob/master/01_Bayesian_Meta-Optimization.ipynb))


## Videos

There is a [YouTube video](https://www.youtube.com/playlist?list=PL9Hr9sNUjfsl1877BS8m3yt8t_wq2IWji) for each research paper.


## Downloading

It is recommended that you download the whole repository from GitHub,
instead of just downloading the individual Python Notebooks.


### Git

The easiest way to download and install this is by using git from the command-line:

    git clone https://github.com/Hvass-Labs/MetaOps.git

This creates the directory `MetaOps` and downloads all the files to it.

This also makes it easy to update the files, simply by executing this command inside that directory:

    git pull


### Zip-File

You can also [download](https://github.com/Hvass-Labs/MetaOps/archive/master.zip)
the contents of the GitHub repository as a Zip-file and extract it manually.


## How To Run

If you want to edit and run the Notebooks on your own computer, then it is
suggested that you use the [Anaconda](https://www.anaconda.com/download)
distribution with **Python 3.6** (or later) because it has most of the required
packages already installed. Then you type the following commands in a terminal
window:

    cd MetaOps
    conda create --name metaops python=3.6
    source activate metaops
    pip install -r requirements.txt

Now you can run the Notebooks by typing this command:

    jupyter notebook


### Run in Google Colab

If you do not want to install anything on your own computer, then the Notebooks
can be viewed, edited and run entirely on the internet by using
[Google Colab](https://colab.research.google.com).
You can click the "Google Colab"-link next to the research papers listed above.
You can view the Notebook on Colab but in order to run it you need to login using
your Google account.
Then you need to execute the following commands at the top of the Notebook,
which clones MetaOps to your work-directory on Colab and installs the required
packages.

    import os
    work_dir = "/content/MetaOps/"
    if os.getcwd() != work_dir:
        !git clone https://github.com/Hvass-Labs/MetaOps.git
    os.chdir(work_dir)
    !pip install -r requirements.txt


## License (MIT)

These Python Notebooks and source-code are published under the [MIT License](https://github.com/Hvass-Labs/MetaOps/blob/master/LICENSE)
which allows very broad use for both academic and commercial purposes.

You are very welcome to modify and use the source-code in your own project.
Please keep a link to the [original repository](https://github.com/Hvass-Labs/MetaOps).
