# Machine Learning Engineer Nanodegree
# Capstone Project
## Project: Predicting In-Hospital Mortality of ICU Patients

1. Clone the repository and navigate to the downloaded folder.
	
	```	
		git clone https://github.com/OrangeWong/predicting_mortality.git
		cd predicting_mortality
	```
	
2. Obtain the necessary Python packages, and switch Keras backend to Tensorflow.  	

	For __Windows__:
	```
		conda env create -f requirements/mlnd_cp.yml
		activate mlnd_cp
		set KERAS_BACKEND=tensorflow
		python -c "from keras import backend"
	```
	
	The libraries used includes:
	- [NumPy](http://www.numpy.org/)
	- [Pandas](http://pandas.pydata.org)
	- [matplotlib](http://matplotlib.org/)
	- [scikit-learn](http://scikit-learn.org/stable/)
	- [psycopg2] (http://initd.org/psycopg/)
	- [iPython Notebook](http://ipython.org/notebook.html)
	- [tensorflow] (https://www.tensorflow.org/)
	- [seaborn] (https://seaborn.pydata.org/)
	- [scipy] (https://www.scipy.org/)
	- [keras] (https://keras.io/)

3. Run notebook in this order: data_extraction, data_wrangling, and data_analysis
	- data_extraction: this notebook is to extract a dataset of mulitvariable time series from MIMIC-III database.
	- data_wrangling: this notebook is to preprocess and clean the extracted time series by removing the outliers and exploring the time series.
	- data_analysis: this notebook is to predict the hospitla dealth in ICU visit based on the first 24 hours of ICU stay data.
	