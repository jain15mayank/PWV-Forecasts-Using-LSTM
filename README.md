## Forecasting Precipitable Water Vapor Using LSTMs

With the spirit of reproducible research, this repository contains all the codes required to produce the results in the manuscript: 

> Jain, M., Manandhar, S., Lee, Y., Winkler, S. and Dev, S.(2020). Forecasting Precipitable Water Vapor Using LSTMs. In: International Symposium onAntennas and Propagation and North American Radio Science Meeting. IEEE. 


The work is done using the Google Colab Framework (with GPU).

## Scripts

+ `read_matfile.py`: reads the matlab mat file that contains the weather station recordings for the year 2010.
+ `pwv_main.ipynb`: main program. Currently, it loads the data, and returns the following numpy arrays of the weather station recordings. This is followed by LSTM training for PWV forecast.
	+ `timestamp`: datetime object
	+ `doy`: day of the year
	+ `hour`: hour of the day
	+ `minute`: minute of the day
	+ `temperature`: temperature
	+ `solar_radiation`: solar radiation
	+ `relative_humidity`: relative humidity
	+ `rain`: rain 
	+ `dew_point_temp`: dew point temperature
	+ `pwv`: precipitable water vapor
+ `test_model.ipynb`: main program. This is to load the trained model and produce results for PWV forecasting.
+ `pwv_lstm.h5`: Trained LSTM model - H5PY file

# Note:
The dataset used in this project can not be disclosed due to external reasons. However, one may feel to use/modify the code as per the requirement.
