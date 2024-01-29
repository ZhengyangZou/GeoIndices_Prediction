# GeoInices_Prediction
This project provides the predicted AE, AU, AL, and Dst prediction in one to three hours ahead (res: 1 hour), by traning onmiweb data using LSTM method.
Please find the details in the paper "A Forecast Model of Geomagnetic Indices from the Solar Wind Fluids Observations based on Long Short-Term Memory Neural Network" under review in Physics of Fluids.
The predicted values are described below.
# 1. For the files in folder "One-step":
   Columns 1-3 -> year, doy, hour 
   
   column 4   -> ground truth (observations)
   
   columns 5-10 -> predictions by using the length input time series 3, 6, 9, 12, 15, 18 hours.
   
# 2. For the files in folder "One-To-Three-step":
   Columns 1-3 -> year, doy, hour
   
   columns 4-6 -> ground truth (observations), values before 1 hour, and values before 2 hours (time-shifted)
   
   columns 7-9 -> one-hour, two-hour, and three-hour predictions by using the length input time series 18 hours.
   
# 3. For the files in folder "Out-of-Sample":
   columns 1-3 -> year, doy, hour
   
   column 4   -> Out-of-Sample ground truth (observations) using replaced AE, AU, and AL values from lasp.colorado.edu/home/ personnel/xinlin.li
   
   columns 5-10 -> Out-of-Sample predictions by using the length input time series 3, 6, 9, 12, 15, 18 hours.
   
