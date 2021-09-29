# MP6D: An RGB-D Dataset for Metal Parts’ 6D Pose Estimation
Information
===========

This is the MP6D dataset [1] for 6D object pose estimation.
It contains 20 videos (6,000 frames in total) of 5 metal parts in real scenes and 20,000 synthetic images, each of which is partially affected by occlusion, illumination changes,
and other factors.
## Instance models and CAD models of 5 objects.

(a) Five metal parts with oxidized aluminum alloy surface. (b) CAD models of the metal parts.
<div align=center><img width="50%" src="src/fig1.png"/></div>

## Real and rendered scenes

The dataset contains 3 real scenes and 20 synthesis scenes. (a), (b), (c) and (d) represent the examples of
the real scenes. (e), (f), (g) and (h) represent the examples of the synthesis scenes.
<div align=center><img width="70%" src="src/fig2.png"/></div>

Basic Usage
===========

## The description of the directories in this package:

1. cameras. The camera parameters used to capture the videos. 
2. data. The 20 videos in the dataset.
3. data_syn. 20,000 synthetic images of the 5 objects.
4. image_sets. Separation of the videos into training set (train.txt) and the testing set (test.txt).
6. models_cad. 5 CAD models of Ply format.

## The description of the Archive  in the directories:

The data of each frame is composed of RGB image, Depth image, Mask image, xxbox.txt and xxx.mat. where xxbox.txt represents the bounding box of the target in the figure. The content data of xxx.mat is as follows：  

1.center: 2D location of the projection of the 3D model origin in the image.      
2.cls_indexes: class labels of the objects.   
3.factor_depth: divde the depth image by this factor to get the actual depth vaule.  
4.intrinsic_matrix: camera intrinsics.  
5.poses: 6D poses of objects in the image.  
<div align=center><img width="50%" src="src/fig3.png"/></div>  

Download
===========

The data can be downloaded as a set of zip archives [here](https://koawere-my.sharepoint.com/:u:/g/personal/yhan_f_svip_gq/EaJdVKHnU3ZIl0HbuqS62BEBQFzj4S2L_Udc87_nHnVwwg?e=K8J6gV).





