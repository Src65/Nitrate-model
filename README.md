# Nitrate-model
Modeling nitrate load from a tidally influenced watershed 

Overview
This project involves modeling nitrate load from a tidally influenced watershed. Specifically, it estimates the annual nitrate load for the Moro Cojo Slough in Moss Landing, CA. The data was autonomously monitored using a station owned and operated by the Central Coast Wetlands Group (CCWG), equipped with a SonTek ADCP and a Sea-Bird SUNA nitrate sensor. Due to occasional station downtime, the model also incorporates tide data from NOAA station 9413450 to estimate watershed discharge and fill the data gaps.

Project Details
Watershed: Moro Cojo Slough, Moss Landing, CA
Sensors: SonTek ADCP, Sea-Bird SUNA nitrate sensor
Tide Data: NOAA station 9413450
Objective: Estimate annual nitrate load

Libraries Used
The following libraries were used in this project:

import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
from scipy import stats
%matplotlib notebook

from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestRegressor
from sklearn.metrics import mean_squared_error
from sklearn.impute import SimpleImputer
