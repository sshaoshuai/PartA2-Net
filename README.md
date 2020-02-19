# From Points to Parts: 3D Object Detection from Point Cloud with Part-aware and Part-aggregation Network

This repository is the PyTorch implementation of our TPAMI paper [[arXiv]](https://arxiv.org/abs/1907.03670).

**Authors**: [Shaoshuai Shi](https://sshaoshuai.github.io/), [Zhe Wang](https://wang-zhe.me/), [Jianping Shi](http://shijianping.me/), [Xiaogang Wang](http://www.ee.cuhk.edu.hk/~xgwang/), [Hongsheng Li](http://www.ee.cuhk.edu.hk/~hsli/).



## Introduction
In this work, we propose the part-aware and aggregation neural network (PartA2-Net). The whole framework consists of the part-aware stage and the part-aggregation stage. Firstly, the part-aware stage for the first time fully utilizes free-of-charge part supervisions derived from 3D ground-truth boxes to simultaneously predict high quality 3D proposals and accurate intra-object part locations. The predicted intra-object part locations within the same proposal are grouped by our new-designed RoI-aware point cloud pooling module, which results in an effective representation to encode the geometry-specific features of each 3D proposal. Then the part-aggregation stage learns to re-score the box and refine the box location by exploring the spatial relationship of the pooled intra-object part locations. 
At the time of submission (July-9 2019), our PartA2-Net outperforms all existing 3D detection methods and achieves new state-of-the-art on KITTI 3D object detection [learderbaord](http://www.cvlibs.net/datasets/kitti/backups/2019_10_08_10_46_41_object_3d.html) by utilizing only the LiDAR point cloud data.

![teaser](https://sshaoshuai.github.io/content/images/PartA2_v2.png)

## Code
The code will be released soon.

## Citation
If you find this work useful in your research, please consider cite:
```
@article{shi2019part,
    title={From Points to Parts: 3D Object Detection from Point Cloud with Part-aware and Part-aggregation Network},
    author={Shi, Shaoshuai and Wang, Zhe and Shi, Jianping and Wang, Xiaogang and Li, Hongsheng},
    journal={arXiv preprint arXiv:1907.03670},
    year={2019}
}
```
