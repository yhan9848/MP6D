# MP6D: An RGB-D Dataset for Metal Parts’ 6D Pose Estimation
Information
===========

This is the MP6D dataset [1] for 6D object pose estimation.
It contains 20 videos (6,000 frames in total) of 5 metal parts in real scenes and 20,000 synthetic images, each of which is partially affected by occlusion, illumination changes,
and other factors.
<div align=center><img width="100%" src="figs/FFB6D_overview.png"/></div>


Basic Usage
===========

The description of the directories in this package:

1. cameras. The camera parameters used to capture the videos. 
2. data. The 20 videos in the dataset.
3. data_syn. 20,000 synthetic images of the 5 MP6D objects.
4. image_sets. Separation of the videos into training set (train.txt) and the testing set (test.txt).
6. plymodels. 3D models of the 5 MP6D objects.


