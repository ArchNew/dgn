# OPEC-Net
[Peeking into occluded joints: A novel framework for crowd pose estimation](https://arxiv.org/pdf/2003.10506.pdf)
(ECCV2020)

# Citation
If you find our works useful in your reasearch, please consider citing:  
```
@article{qiu2020peeking,
  title={Peeking into occluded joints: A novel framework for crowd pose estimation},
  author={Qiu, Lingteng and Zhang, Xuanye and Li, Yanran and Li, Guanbin and Wu, Xiaojun and Xiong, Zixiang and Han, Xiaoguang and Cui, Shuguang},
  journal={arXiv preprint arXiv:2003.10506},
  year={2020}
}

```

# OCPose

## About OCPose
We build a new dataset, called Occluded Pose(OCPose), that includes more heavy occlusions to evaluate the MPPE. It contains challenging invisible jointsand complex intertwined human poses.


Dataset | Total | IoU>0.3 | IoU>0.5 | IoU>0.75 | Avg IoU
:--:|:--:|:--:|:--:|:--:|:--:
CrowdPose | 20000 | 8704(44%) | 2909(15%) | 309(2%) | 0.27  
COCO2017 | 118287 | 6504(5%) | 1209(1%) | 106(<1%) | 0.06  
MPII | 24987 | 0 | 0 | 0 | 0.11
OCHuman | 4473 | 3264(68%) | 3244(68%) | 1082(23%) | 0.46  
OCPose | 9000 | 8105(**90%**) | 6843(**76%**) | 2442(**27%**) | **0.47**

## Download

[Images](https://drive.google.com/file/d/1oQ1_epocYgvlha4eowt1FS-5f89XU7xw/view?usp=sharing)  
[Annotations](https://drive.google.com/file/d/1z8xlN56x9aKve4YSEudYJOJOPt4YaC7H/view?usp=sharing)


# Quick Start under CrowdPose Datasets

## Download Datasets
[COCO2017](https://cocodataset.org)  
[CrowdPose](https://github.com/Jeff-sjtu/CrowdPose)  

## Download processed annotations

pls, Download annotations processed by sampling rules according to our paper  
[train_process_datasets](https://drive.google.com/file/d/1WlZETQuOJWWARos8nnQw9XRamsTRTrrA/view?usp=sharing)  
[test_process_datasets](https://drive.google.com/file/d/1WlZETQuOJWWARos8nnQw9XRamsTRTrrA/view?usp=sharing)  

## Pretrain module
Here, we employ top-down module([Alphapose+](https://github.com/MVIG-SJTU/AlphaPose/tree/pytorch) based on pytorch) as our initial module.  
The pretrain checkpoints trained by official codes could be download as following:  
[SPPE](https://drive.google.com/file/d/1Wcf5CWYGeMsfKn77Pu5wk6GpwEIScY2q/view?usp=sharing)  
[yolov3](https://drive.google.com/file/d/1IAtLxnOkE5DkTJ5Lsi7kLLU-edAgzaw_/view?usp=sharing)  


