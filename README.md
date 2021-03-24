# Climate Forecasting with Long Short Term Memory ntworks

The purpose of this model is to apply the Long Short Term Memory networks in order to predict the average temperature trend in Italy. The dataset comes from [Kaggle.](https://www.kaggle.com/berkeleyearth/climate-change-earth-surface-temperature-data). For additional information about this Models you can read my article on Towards Data Science [here]().

## Description of the data that I used

- Date: starts in 1750 for average land temperature and 1850 for max and min land temperatures and global ocean and land temperatures
- LandAverageTemperature: global average land temperature in celsius
- LandAverageTemperatureUncertainty: the 95% confidence interval around the average

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

**Prediction vs original data
<img src="https://cdn-images-1.medium.com/max/1320/1*P0_MrCDm1aqzRU5GQ8t4pw.png">






