# Inspur_DABNet4D
This method performs 3D object detection in the BEV space using images from multiple cameras. It first predicts the depth of each camera and then projects the extracted image features into BEV space. Moreover, it utilizes temporal information by aligning the BEV features. We use ConvNeXt-Base pre-trained on ImageNet as the image backbone and train the model for 24 epochs with CBGS.

Results
3D Object Detection (on nuScenes test)
Model	mAP	NDS
Inspur-DABNet4D-1600	53.21	62.37
#3D Object Detection (on nuScenes val)
#Model	mAP	NDS
#Inspur-MASTER-704	35.91	49.75
Get Started
Environment
This implementation is build upon mmdetection3d, please follow the steps in install.md to prepare the environment.

Data
Please follow the official instructions of mmdetection3d to process the nuScenes dataset.(https://mmdetection3d.readthedocs.io/en/latest/datasets/nuscenes_det.html)

Acknowledgement
Many thanks to the following open-source projects:

mmdetection3d
Reference
@{author={Zhaoyun, Gongzhan, Lijun, Zhuhong}}
