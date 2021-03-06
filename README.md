# Climate Forecasting with Long Short Term Memory Networks

The purpose of this model is to apply the Long Short Term Memory networks in order to predict the average temperature trend in Italy. The dataset comes from [Kaggle](https://www.kaggle.com/berkeleyearth/climate-change-earth-surface-temperature-data). For additional information about this Model you can read my article  [here](https://towardsdatascience.com/forecasting-climate-change-in-italy-with-long-short-term-memory-networks-eef4990d7b8c?sk=f05e31c06bd24766a7e66f108f2fd86e) and the entire code is also availabe [here.](https://colab.research.google.com/github/moryba/Climate_Analysis/blob/main/climate_analysis.ipynb)

## Description of the data that I used

- Date: starts in 1750 for average land temperature and 1850 for max and min land temperatures and global ocean and land temperatures
- LandAverageTemperature: global average land temperature in celsius
- LandAverageTemperatureUncertainty: the 95% confidence interval around the average
- Country : names of the countries with data available year by year

## Usage
```python
import pandas as pd
import plotly.express as px
from copy import copy
import matplotlib.pyplot as plt
import numpy as np
import seaborn as sns
from sklearn.model_selection import train_test_split
from sklearn.metrics import r2_score
from sklearn.preprocessing import MinMaxScaler
import tensorflow as tf
from tensorflow import keras
import plotly.offline as py
import plotly.express as px
import plotly.graph_objects as go
```

## Exploratory Data Analysis

**Average Global Temperature**
<img src="https://media.giphy.com/media/fmfeu7MeFKwsQsJ56J/giphy.gif" width="1300">

**Average Temperature from 1743 to 2013**
<img src="https://media.giphy.com/media/48glxMtr0mESV2qgJP/giphy.gif" width="1300">

**Temperature of Italy from 1743 to 2013 for each month**
<img src="https://media.giphy.com/media/xZbonSHrZovvFHylFc/giphy.gif" width="1300">
  
## Performance of the model

**Prediction vs original data**
<img src="https://cdn-images-1.medium.com/max/1320/1*P0_MrCDm1aqzRU5GQ8t4pw.png">


## Additional information
It is also possible to view the code on Google Colab [here.](https://colab.research.google.com/github/moryba/Climate_Analysis/blob/main/climate_analysis.ipynb)




