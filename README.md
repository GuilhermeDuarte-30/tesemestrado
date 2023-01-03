# tesemestrado

MilhoMaxcorreto->maize with a pre-selection of the time series with the 10% highest values at the global maximum of all the time series for that crop

Milhocorreto90->maize with a pre-selection of the time series with a Pearson correlation higher or equal to 0.9 with the Kc

Milhocorreto->maize with no pre-selection

KcNDVI->Kc values in each development stage

KcTime->duration of each development stage


#Methodology for each notebook:

1.Reading the files

2.Pre-processing of the data (linear interpolation to remove NaN, Savitzky-Golay filter to remove the noise and Pearson correlation to choose the best period for each series)

3.Using a pre-selection in MilhoMaxcorreto and Milhocorreto90 cases

4.Create a train and test set

5.Use Mean and K-means to create a single time series

6.Fit the time series to linear and polynomial regression

7.Evaluate the models (R2 and RMSE)
