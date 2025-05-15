# [Deep Discriminative Boundary Hashing for Cross-modal Retrieval](https://ieeexplore.ieee.org/document/11003934)
This paper is accepted for publication with TCSVT.


## Training

### Processing dataset
Refer to [DSPH](https://github.com/QinLab-WFU/DSPH)

### Download CLIP pretrained model
Pretrained model will be found in the 30 lines of [CLIP/clip/clip.py](https://github.com/openai/CLIP/blob/main/clip/clip.py). This code is based on the "ViT-B/32".

You should copy ViT-B-32.pt to this dir.

### Start

After the dataset has been prepared, we could run the follow command to train.
> python main.py --is-train --dataset coco --caption-file caption.mat --index-file index.mat --label-file label.mat --lr 0.001 --output-dim 64 --save-dir ./result/coco/64 --clip-path ./ViT-B-32.pt --batch-size 128

### Citation
@ARTICLE{11003934,  
  author={Qin, Qibing and Huo, Yadong and Zhang, Wenfeng and Huang, Lei and Nie, Jie},  
  journal={IEEE Transactions on Circuits and Systems for Video Technology},  
  title={Deep Discriminative Boundary Hashing for Cross-modal Retrieval},  
  year={2025},  
  volume={},  
  number={},  
  pages={},  
  doi={10.1109/TCSVT.2025.3570128}}
