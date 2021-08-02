
Skills I Developed:

Time Series Prediction - LSTM

Project - Predict the hourly rain gauge total

This is a time series prediction task: I am given snapshots of polarimetric radar values and asked to predict the hourly rain gauge total.

First, login to Kaggle and download the dataset. https://www.kaggle.com/c/how-much-did-it-rain-ii/data

Now you need to use an LSTM model to predict the hourly rain gauge total.

Data description

To understand the data, you have to realize that there are multiple radar observations over the course of an hour, and only one gauge observation (the 'Expected'). That is why there are multiple rows with the same 'Id'.

The columns in the datasets are:

Id: A unique number for the set of observations over an hour at a gauge.

minutes_past: For each set of radar observations, the minutes past the top of the hour that the radar observations were carried out. Radar observations are snapshots at that point in time.

radardist_km: Distance of gauge from the radar whose observations are being reported.

Ref: Radar reflectivity in km

Ref_5x5_10th: 10th percentile of reflectivity values in 5x5 neighborhood around the gauge.

Ref_5x5_50th: 50th percentile

Ref_5x5_90th: 90th percentile

RefComposite: Maximum reflectivity in the vertical column above gauge. In dBZ.

RefComposite_5x5_10th

RefComposite_5x5_50th

RefComposite_5x5_90th

RhoHV: Correlation coefficient (unitless)

RhoHV_5x5_10th

RhoHV_5x5_50th

RhoHV_5x5_90th

Zdr: Differential reflectivity in dB

Zdr_5x5_10th

Zdr_5x5_50th

Zdr_5x5_90th

Kdp: Specific differential phase (deg/km)

Kdp_5x5_10th

Kdp_5x5_50th

Kdp_5x5_90th

Expected: Actual gauge observation in mm at the end of the hour.
