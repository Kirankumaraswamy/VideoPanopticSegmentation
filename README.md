# VideoPanopticSegmentation

## To prepare the kitti dataset 
1) set the env to kitti dataset path EG: KITTI_DATASET=/home/abcd/datasets/kitti/
2) run the file VideoPanopticSegmentation/detectron2/detectron2/data/datasets/createKittiPanopticImages.py

## To train the model use kitti config yml path as a parameter
EG: --config-file /home/abcd/VideoPanopticSegmentation/detectron2/projects/Panoptic-DeepLab/configs/Cityscapes-PanopticSegmentation/panoptic_deeplab_R_52_os16_mg124_poly_90k_bs32_crop_512_1024_dsconv.yaml --resume MODEL.WEIGHTS /home/abcd/VideoPanopticSegmentation/detectron2/projects/Panoptic-DeepLab/model_final_23d03a.pkl
Note: Don't forget to set env DETECTRON2_DATASETS. EG: DETECTRON2_DATASETS=/home/abcd/datasets