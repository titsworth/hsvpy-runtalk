# Analyzing Run Data with IPython, gpxpy, and pandas.

This talk will provide an example based introduction to IPython and pandas. Specifically we will analyze a bunch of run data exported from popular run tracking websites, such as Runkeeper and MapMyRun. We will also hit on some visualization products in the Python scientific stack, such as matplotlib and seaborn for visualizations.

## Get the notebooks

The repository for my talk is located here:

[https://github.com/titsworth/talks](https://github.com/titsworth/talks)

Once you clone this repository, you can start setting up your environment

## Getting set up

For simplicity, I suggest installing the Anaconda Python disctributions, which comes with many of the Python scientific packages pre-built. 

Download Anaconda at [http://continuum.io/downloads](http://continuum.io/downloads).

Once anaconda is installed, you can set up a new conda environment (sort of like a Python virtualenv). I have provided a conda environment file to set up the exact environment I was working in while building the notebooks for this talk.

    >> conda create -n runtalk --file environment.conda

 This should get most the appropriate packages for this talk and set you up in a new environment. To swith co this environment, run the following command.

    >> source activate runtalk  # mac/linux
    X:\> activate runtalk       # windows

 You will also need to install a few extra packages with plain ol' pip since they are not controlled by the conda team at this point

     >> pip install -r requirements.txt

## IPython V2.0

 One last item, I am currently usinf IPython V2.0 which is still in development. Most of the talk can be done with the IPython that comes bundled with Anaconda, but if you want to follow along completely, here is how to get set up with the latest development version of IPython. (Remember to switch to your runtalk environment if you are not already there)

 	>> git clone https://github.com/ipython/ipython.git
 	>> cd ipython
 	>> python setup.py install

