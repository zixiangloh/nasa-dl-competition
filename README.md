NASA Deep Learning Competition  
NASA Airathon: Predict Air Quality (Particulate Tracking)  
https://www.drivendata.org/competitions/88/competition-air-quality-pm/  
  
Instruction:  
1. Run download_data.ipynb to download the training dataset. (Needs AWS CLI). See  
https://drivendata-prod.s3.amazonaws.com/data/88/public/airathon_download_instructions_pm25_yMi34QG.txt?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARVBOBDCYZDRLDSRZ%2F20220321%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220321T045235Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=97cb5c1e34c6dfdf160d61a3765a5f0a456cc432b36ee69c7d40d39d0956d7fa    
3. Preprocess the data with the nasa_airathon_data_preprocessor_run\* scripts.  
4. Models and training are all in nasa_airathon.ipynb.  
  
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
