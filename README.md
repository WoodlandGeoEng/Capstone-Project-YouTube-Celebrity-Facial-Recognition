# Capstone-Project-YouTube-Celebrity-Facial-Recognition
Perform Facial Recognition on YouTube Celebrities

This dataset is a processed version of the YouTube Faces Dataset, that contained short videos of celebrities that are publicly available and downloaded from YouTube. There are multiple videos of each celebrity (up to 6 videos per celebrity). The original videos were cropped around the faces and only 240 consecutive frames were kept for each original video. 
The dataset is available here: https://www.kaggle.com/selfishgene/youtube-faces-with-facial-keypoints

This is the **2nd of 3 Notebooks** containing a comparison of possible models built to perform facial recognition of the facial landmarks provided in teh dataset.

**Notebook 1: YouTubeFacialRecognition.ipynb**  
    - Contains all the mothods used on the subset data (youtube_faces_with_keypoints_small.csv) provided on Kaggle)
**Notebook 2: YouTubeFacialRecognitionBig.ipynb** 
    - Contains clustering and classification methods on the full dataset (youtube_faces_with_keypoints_large.csv)
**Notebook 3: YouTubeFacialRecognitionBig-ANNs.ipynb** 
    - Contains roughly optimized neural networks on both the 2D and 3D landmarks

Supporting documents: 
- a .csv files containing the full list and a subset list of the file names and number of frames for each video file (big set)
- the corresponding .npz files containing the rgb color image frame, the bouding box and 2D and 3D landmark coordinates
- my stacked cleverly named 'export_dataframe.csv' file with each frame given a line in the table with the name of the person, the frame number and label encoding, to save you some time!
- a model final model for a small dataset (best_modelsmall7.h5) and a model for the large dataset (best_model_3D4.h5)

References:
Lior Wolf, Tal Hassner and Itay Maoz 
Face Recognition in Unconstrained Videos with Matched Background Similarity. 
IEEE Conf. on Computer Vision and Pattern Recognition (CVPR), 2011. (pdf)

2D and 3D keypoints, from the following paper: 
<br>Adrian Bulat and Georgios Tzimiropoulos. 
How far are we from solving the 2D & 3D Face Alignment problem? 
(and a dataset of 230,000 3D facial landmarks), arxiv, 2017. (pdf)
