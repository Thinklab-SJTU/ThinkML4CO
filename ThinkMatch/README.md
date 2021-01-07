# Repository of Deep Graph Matching

This repository contains pytorch source code of deep graph matching 
methods: 

* **GMN** Andrei Zanfir and Cristian Sminchisescu, "Deep Learning of 
Graph Matching." CVPR 2018.
* **PCA** Runzhong Wang, Junchi Yan and Xiaokang Yang, "Learning 
Combinatorial Embedding Network for Deep Graph Matching."
* **NGM** Runzhong Wang, Junchi Yan and Xiaokang Yang, "Neural Graph 
Matching Network: Learning Lawler’s
Quadratic Assignment Problem."

## Get started

1. Install and configure pytorch 1.1+ (with GPU support)
1. Install ninja-build: ``apt-get install ninja-build``
1. Install python packages: ``pip install tensorboardX scipy easydict 
pyyaml``
1. If you want to run experiment on Pascal VOC Keypoint dataset:
    1. Download VOC2011 and make sure it looks like 
``data/PascalVOC/VOC2011``
    1. Download keypoint annotation from [this 
link](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/shape/poselets/voc2011_keypoints_Feb2012.tgz) 
and make sure it looks like ``data/PascalVOC/annotations``
    
## Training

Run training and evaluation

``python train_eval.py --cfg your_config_file`` 

and replace ``your_config_file`` by path to your configuration file. 
Default configuration files are stored in``experiments/``.

