## *A Two-Stream Approach to Anomaly Detection in Surveillance Videos*

### Abstract:
Surveillance cameras can be found everywhere in today’s society, and their use is continuously growing. With that, the need for quality review of these videos has increased. However, manual review of every video is almost impossible and an automated solution has become more attractive. So, we’re proposing a solution to this by finding anomalies in surveillance videos using deep learning. Our technique utilizes MIL (Multiple Instance Learning) with a two-stream network. One stream consists of RGB (Red Green Blue) videos and the other stream utilizes background reduction and optical flow. Our results show the use of a Two-Stream method has slightly improved anomaly detection as well as greatly reducing false flags when compared to existing methods.

### Illustration:
<img src="https://github.com/anantalp/AnomalyDetection/blob/main/code/figures/fig1.PNG">

### Comparison with state-of-the-art results:
<img src="https://github.com/anantalp/AnomalyDetection/blob/main/code/figures/fig2.PNG">

### Dataset:
The dataset can be downloaded from the following link:
https://webpages.uncc.edu/cchen62/dataset.html

### The implementation is tested using:
1) Keras version 1.1.0
2) Theano 1.0.2
3) Python 3
4) Ubuntu 16.04

### Implementation Details:
1) We used C3D-v1.0 (https://github.com/facebook/C3D) with default settings as a feature extractor. 
2) Training_AnomalyDetecor_public.py is to Train Anomaly Detection Model. Testing_Anomaly_Detector_public.py is to test trained Anomaly Detection Model.
3) Save_C3DFeatures_32Segments is to save already computed C3D features for the whole video into 32 segment features.
4) weights_L1L2.mat: It contains the pre-trained weights for the model ‘model.json’.
5) Demo_GUI: We have provided a simple GUI which can be used to see results of our approach on sample videos.
6) SampleVideos: This folder contains C3D features (32 segments) for sample videos. It order to see testing results for the features in this folder, please copy the corrosponding videos in the same folder.
7) Plot_All_ROC:  This code can be use to plot the ROC results reported in the paper. The data to plot ROCs of methods discussed in the paper can be found in folder Paper_Results.
8) Temporal_Anomaly_Annotation.txt contains ground truth annotations of the testing dataset.




