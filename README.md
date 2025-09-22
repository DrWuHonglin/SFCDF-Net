# SFCDF-Net
## SFCDF-Net: Enhancing Multi-modal Semantic Segmentation via Spatial-Frequency Collaborative Filtering

<p align="center">
  <img src="https://github.com/DrWuHonglin/SFCDF-Net/blob/main/images/framework.png" width="900" height="450">
</p>

This repository contains the official implementation of SFCDF-Net, a novel network for multimodal semantic segmentation.

- Achieves efficient and precise multimodal remote sensing semantic segmentation
- SFCDF-Net: A dual-stream multimodal semantic segmentation network with a multilevel fusion strategy.
- A CCSI module is proposed to leverage selective interactions and attention-based enhancement for initial spatial refinement, effectively narrowing the modality gap and guiding subsequent frequency domain filtering.
- We propose a DSF to dynamically filter and select informative frequency components in a data-driven manner, enabling effective cross-modal frequency domain interaction and noise suppression
  
## Results

1. SFCDF-Net achieves competitive results on the following datasets:
- Vaihingen: 83.94% mIoU
- Potsdam: 86.02% mIoU
2. We provide visualizations of our results on the Vaihingen and Potsdam datasets:
<p align="center">
  <img src="https://github.com/DrWuHonglin/SFCDF-Net/blob/main/images/invaihingen.png" width="800" height="450">
</p>
<p align="center">
  <img src="https://github.com/DrWuHonglin/SFCDF-Net/blob/main/images/inposdam.png" width="800" height="450">
</p>

## Installation
1. Requirements
   
- Python 3.10.15	
- CUDA 12.1
- torch==1.13.0+cu117
- torchvision==0.14.0+cu117
- tqdm==4.66.4
- numpy==1.23.5
- pandas==2.0.1
- ipython==8.12.3

## Demo
To quickly test the SFCDF-Net with randomly generated tensors, you can run the demo.py file. This allows you to verify the model functionality without requiring a dataset.
1. Ensure that the required dependencies are installed:
```
pip install -r requirements.txt
```
2. Run the demo script:
```
python demo.py
```

## Datasets
All datasets including ISPRS Potsdam, ISPRS Vaihingen can be downloaded [here](https://github.com/open-mmlab/mmsegmentation/blob/main/docs/en/user_guides/2_dataset_prepare.md#prepare-datasets).
