NASA Deep Learning Competition  
NASA Airathon: Predict Air Quality (Particulate Tracking)  
https://www.drivendata.org/competitions/88/competition-air-quality-pm/  
  
Instruction for main HDF model:  
1. Run download_data.ipynb to download the training dataset. (Needs AWS CLI). See https://www.drivendata.org/competitions/88/competition-air-quality-pm/data/  
2. Preprocess the data with the nasa_airathon_data_preprocessor_run\* scripts.  
3. Models and training are all in nasa_airathon_main.ipynb.  
  
Other items:  
1. The nasa_airathon_main_7feature_per_layer.ipynb model is a 7 feature model instead of 4. Performance was similar.  
2. The Code_From_Tutorial.ipynb code is for testing code given by the tutorial on the website. See: https://www.drivendata.co/blog/predict-pm25-benchmark/  
3. The Weather_Model.ipynb code is our attempt at using auxiliary data to help improve the model. We were trying to see if this can help solve a fundamental problem with missing features (NaN).  
4. The Exploring_NC_Files.ipynb is our attempt at using the \*.nc files. This didn't pan out well because the submission format didn't have any rows/grids/datetimes that use the \*.nc files.  
  
Things provided:  
1. submission_format.csv is provided for submission to the competition website. Must be the same format  
2. grid_metadata.csv, train_labels.csv and pm25_satellite_metadata.csv is provided to us as part of the competition.  
3. submission_model_39_r2_val_0p5273908363822994.csv is the highest R^2 cross validation score model we have (and also the one we submitted with 0.56 R2).  
  
Repo & Data Structure:  
The repo will look like so after running the download_data script and the preprocessing scripts  
repo  
\|-- train/\*.hdf,\*.nc  
\|-- test/\*.hdf,\*.nc  
\|-- train_processed_pickles/\*.pbz2  
\|-- test_processed_pickles/\*.pbz2  
  
Contributors:  
zl3021@columbia.edu  
jwb2168@columbia.edu  
