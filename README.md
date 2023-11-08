# Deepdake-Detection-using-PPG-Maps
FaceForensics++ data set is used for training and evaluation of our approach.  
PPG maps are generated for each segment(of 128 frames) of a video. Video is classified based on majority votng of it's segment predictions.  
Previously Chrominace channel based PPG maps were considered for detecting deepfake videos, But later studies revieled that R,V,Y,B,G channels shows higher difference between real and fake frames' faces.  
Among those 5 channels B and G are redundant channel higher correlations with V and Y, so R,V,Y channels are considered for generating a PPG map.  
'fc_fake_rvy.ipynb' and 'fc_real_rvy.ipynb' creates the required dataset of PPG maps for training CNN model.  
From the PPG maps generated neraly 70% is used for training and 30% data is used for testing.  
CNN model gives the segment accuracy of 95% and based on majority voting of segment prediction our approach gave video accuracy of 96.3%.  
