# MP6D
An RGB-D Dataset for Metal Parts’ 6D Pose Estimation
Information
===========

This is the YCB-Video dataset [1] for 6D object pose estimation.
It provides accurate 6D poses of 21 objects from the YCB dataset [2] 
observed in 92 videos with 133,827 frames.

This project was funded in part by Siemens and by NSF
STTR grant 63-5197 with Lula Robotics.


How to Cite
===========

@article{xiang2017posecnn,
author    = {Xiang, Yu and Schmidt, Tanner and Narayanan, Venkatraman and Fox, Dieter},
title     = {PoseCNN: A Convolutional Neural Network for 6D Object Pose Estimation in Cluttered Scenes},
journal   = {arXiv preprint arXiv:1711.00199},
year      = {2017}
}


Basic Usage
===========

The description of the directories in this package:

1. cameras. The camera parameters used to capture the videos. asus-uw.json for video 0000 ~ 0059, asus-cmu.json for video 0060 ~ 0091.
2. data. The 92 videos in the dataset.
3. data_syn. 80,000 synthetic images of the 21 YCB objects.
4. image_sets. Separation of the videos into training set (train.txt) and the testing set (val.txt, keyframe.txt).
5. keyframes. Keyframe indexes of the 12 testing videos.
6. models. 3D models of the 21 YCB objects.
7. pairs. Stereo pair indexes of the 12 testing videos.
8. poses. All the 6D poses of the 21 YCB objects in the dataset (quaternion + translation).

References
==========

[1] Y. Xiang, T. Schmidt, V. Narayanan and D. Fox.
PoseCNN: A convolutional neural network for 6D object pose estimation in cluttered scenes. In arXiv:1711.00199, 2017.

[2] B. Calli, A. Singh, A. Walsman, S. Srinivasa, P. Abbeel, and A. M. Dollar. The YCB object and model set: Towards common benchmarks
for manipulation research. In International Conference on Advanced Robotics (ICAR), pp. 510–517, 2015.
