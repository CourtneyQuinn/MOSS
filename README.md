# Exploring predictors of Tropical Cyclone strength

We are interested in variables that can be used as predictors for changes in cyclone strength.  We use output from an axisymmetric numerical model used to simulate a tropical cyclone (Bryan and Rotunno 2009).  The model is based on a compressible nonhydrostatic cloud model (CM1, Bryan and Fritsch 2002) with dissipative heating, and reversible saturated conditions.  We consider maximum tangential velocity and minimum surface pressure as predictands for strength.  The predictors of interest are minimum radial velocity, maximum vertical velocity, and maximum diabetic heating.  We create a simple regression model and compare to the model output.

## Prerequisites

Python

## Built With

* [JupyterLab](http://jupyterlab.readthedocs.io/en/stable/) - The web framework used

## Notebooks relating to the project outputs

AC_exploredata_updated.ipynb - Visualizing data and Creating a Regression model

CQ_EWS.ipynb - Calculating Early Warning Signals for Eyewall Replacement Cycle

## Authors

* **Courtney Quinn** - *Initial work* - [CourtneyQuinn](https://github.com/CourtneyQuinn)
* **Michelle Spruce** - *Initial work* - [MSpruce](https://github.com/MSpruce)
* **Aisawan Chankarn** - *Initial work* - [aisawa20](https://github.com/aisawa20)

See also the list of [contributors](https://github.com/CourtneyQuinn/MOSS/graphs/contributors) who participated in this project.

## Acknowledgments

* EPSRC MPE CDT program
* UK Met Office
* Netherlands eScience center
