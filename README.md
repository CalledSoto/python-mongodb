## Install Anaconda
The simplest way to run the project is by installing [Anaconda] (https://www.anaconda.com/distribution/).

With Anaconda installed correctly, navigate to the project directory
and run:
`` ''
# navigate to the project directory
cd platzi-mongo
# create a new environment
conda create --name platzi-mongo
# activate the environment
conda activate platzi-mongo
# to disable the environment
conda deactivate
`` ''
If you use Python frequently and have a 3.3+ version, you don't need to
Install Anaconda, create a virtual environment with venv or virtualenv and continue with
the step of installing the dependencies.
## Install project dependencies
With the environment activated, install the dependencies:
`` ''
pip install -r requirements.txt
`` ''
## Environment variables necessary to run the project
Make sure to replace the value of PLATZI_DB_URI with the URI of your cluster in MongoDB Atlas
`` ''
export FLASK_APP = platzi-api
export FLASK_ENV = development
export PLATZI_DB_URI = "MONGO-URI"
`` ''

## start platzi-mongo server
`` ''
flask run
`` ''
