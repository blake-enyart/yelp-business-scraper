
# Welcome to the Yelp Business Extraction Notebook!

This project is a that is put together for the express purpose of helping organizations identify all of the existing organizations within a specific radius. This project utilizes the Yelp API and is built completely on a Jupyter Notebook for expediency.

## Getting Started

Prior to configuring your virtualenv, ensure you have [poetry](https://python-poetry.org/) installed globally for your python version. Furthermore, you must also create a Yelp API key to access the Yelp Fusion API which can be done [here](https://www.yelp.com/developers/v3/manage_app)

Once you have created your API key, add this to a `.env` file at the root of this project and name it as follow: `YELP_API_KEY=<API key goes here>`

Create a virtualenv on MacOS and Linux:

```
$ python3 -m venv .venv
```

After the init process completes and the virtualenv is created, you can use the following
step to activate your virtualenv.

```
$ source .venv/bin/activate
```

If you are a Windows platform, you would activate the virtualenv like this:

```
% .venv\Scripts\activate.bat
```

Once the virtualenv is activated, you can install the required dependencies.

```
$ poetry install
```

Get started with the Jupyter Notebook using thi command

```
$ jupyter notebook
```

Enjoy!

## Choosing a location

Use Map Developers (https://www.mapdevelopers.com/draw-circle-tool.php) interface in order to create a point/radius which can then be passed into the `params` variable in this Jupyter Notebook.

## Troubleshooting

It is best practice to ensure that each Jupyter notebook is run within it's own virtual environment. To accomplish this, ensure that `jupyter` and `ipykernel` are uninstalled globally. 

Otherwise this will cause pathing issues in identifying the libraries installed with the commands above. The most likely culprits for this would be a `brew` installation or global `pip` installation.

Just perform the required global uninstallations prior to activating the virtual environment and then perform the steps in the getting started.