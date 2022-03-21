NASA Deep Learning Competition  
NASA Airathon: Predict Air Quality (Particulate Tracking)  
https://www.drivendata.org/competitions/88/competition-air-quality-pm/  
  
Instruction:  
1. Run download_data.ipynb to download the training dataset. (Needs AWS CLI). See https://www.drivendata.org/competitions/88/competition-air-quality-pm/data/  
2. Preprocess the data with the nasa_airathon_data_preprocessor_run\* scripts.  
3. Models and training are all in nasa_airathon_main.ipynb.  
  
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
