# Polyp_segmentation
### Repository of the paper: An efficient real-time polyp segmentation system based on CNNs and transformers on a new comprehensive dataset.

#### This repository contains:
* Implementation of a novel deep learning model to segment the polyp images.
* Dataset file that introduced in the paper.
* Comprehensive dataset includes CVC-300, CVC-ColonDB, CVC-ClinicDB, Kvasir-seg, ETIS-Larib, PolypGen, Neopolyp-small, SUN-SEG, 

## Model implementation  
training:
```
!python tools/train.py configs/custom_config.py <num-of-gpus-to-use> --work-dir /path/to/save/checkpoint
```
    
    
testing:
```
!python tools/test.py configs/custom_config.py <num-of-gpus-to-use> --work-dir /path/to/save/checkpoint
``` 
    
### Requirements  
* pytorch = 1.10.0  
* cuda = 11.1  
* timm = 0.6.7  
* mmcv-full = 1.5.0  

## dataset
##### Download the training and testing dataset from this link: [Google Drive](https://drive.google.com/drive/folders/170354jP6Rwg57u6qcK0u5szO9eWBPgVP?usp=sharing)

dataset folders:  
    
    |-- TrainDataset
    |   |-- images
    |   |-- masks
    |-- TestDataset
    |   |-- CVC-300
    |   |   |-- images
    |   |   |-- masks
    |   |-- CVC-ClinicDB
    |   |   |-- images
    |   |   |-- masks
    |   |-- CVC-ColonDB
    |   |   |-- images
    |   |   |-- masks
    |   |-- ETIS-LaribPolypDB
    |   |   |-- images
    |   |   |-- masks
    |   |-- Kvasir
    |       |-- images
    |       |-- masks


## Our dataset
##### Download the training and testing dataset from this link: [Google Drive](https://drive.google.com/drive/folders/11nER2DP2Fjc18sTDypDmZv6Nbp0p7-Ms?usp=sharing)

dataset folders:  
    
    |-- TrainDataset
    |   |-- images
    |   |-- masks
    |-- TestDataset
    |   |-- images
    |   |-- masks
    

## Comprehensive dataset
##### Download the training and testing dataset from this link: [Google Drive](https://drive.google.com/drive/folders/1cRngyiUuv0Vk7Wj3MAb-JRnunOrbqvpf?usp=sharing)
dataset folders:  
    
    |-- TrainDataset
    |   |-- images
    |   |-- masks
    |-- TestDataset
    |   |-- C5_polypgen
    |   |   |-- images
    |   |   |-- masks
    |   |-- C6_polypgen
    |   |   |-- images
    |   |   |-- masks
    |   |-- C10_ETIS
    |   |   |-- images
    |   |   |-- masks
    |   |-- C13_CVC-300
    |   |   |-- images
    |   |   |-- masks
    |   |-- C14_CVC_ColonDB
    |       |-- images
    |       |-- masks
    |   |-- seen_dataset
    |       |-- C1_polypgen
    |           |-- images
    |           |-- masks
    |       |-- C2_polypgen
    |           |-- images
    |           |-- masks
    |       |-- C3_polypgen
    |           |-- images
    |           |-- masks
    |       |-- C4_polypgen
    |           |-- images
    |           |-- masks
    |       |-- C7_kvasir
    |           |-- images
    |           |-- masks
    |       |-- C8_our_dataset
    |           |-- images
    |           |-- masks
    |       |-- C9_CVC_Clinic
    |           |-- images
    |           |-- masks
    |       |-- C11_neopolyp_small
    |           |-- images
    |           |-- masks
    |       |-- C12_SUN-SEG
    |           |-- images
    |           |-- masks

## Acknowledgement
The implementation is based on [MMSegmentation](https://github.com/open-mmlab/mmsegmentation).

## Citation
Please cite our paper if you find the work useful:
