# EPM-Net
Code for "EPM-Net: Efficient Feature Extraction, Point-pair Feature Matching for Robust 6D Pose Estimation"

<img src="doc/network.png" />

## Requirements
* Open3D==0.16.0
* python==3.7.13
* OpenCV==4.6.0
* Pytorch==1.7.0
* CUDA==11.4

## Downloads
* YCB-Video dataset [[link](https://rse-lab.cs.washington.edu/projects/posecnn/)]
* Preprocesssed LineMOD dataset (refer from DenseFusion) [[link](https://hkustconnect-my.sharepoint.com/personal/yhebk_connect_ust_hk/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fyhebk%5Fconnect%5Fust%5Fhk%2FDocuments%2Fpublically%20shared%20%E5%85%B1%E4%BA%AB%E6%96%87%E4%BB%B6%E5%A4%B9%2F6D%5Fpose%5Fdatasets%2FLinemod%5Fpreprocessed%2Ezip&parent=%2Fpersonal%2Fyhebk%5Fconnect%5Fust%5Fhk%2FDocuments%2Fpublically%20shared%20%E5%85%B1%E4%BA%AB%E6%96%87%E4%BB%B6%E5%A4%B9%2F6D%5Fpose%5Fdatasets&ga=1)]
* Pred mask of HybirdPose on LineMOD Occlusion dataset [[link](https://drive.google.com/file/d/1Jwp-J6opAAvtbMV1ewzhpBLoSjmZoMVJ/view)]

## Train
Train our EPM-Net:

For YCB-Video dataset and LineMOD dataset, run:
```python
python train.py --dataset ycbv --dataset_root path_to_ycbv_dataset
python train.py --dataset linemod --dataset_root path_to_lm_dataset
