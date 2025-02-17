# TLS registration

The methodology behing this research is elaborated in following paper:
```
@article{BEDKOWSKI2023113199,
     title = {Benchmark of multi-view Terrestrial Laser Scanning Point Cloud data registration algorithms},
     journal = {Measurement},
     pages = {113199},
     year = {2023},
     issn = {0263-2241},
     doi = {https://doi.org/10.1016/j.measurement.2023.113199},
     url = {https://www.sciencedirect.com/science/article/pii/S0263224123007637},
     author = {Janusz Będkowski},
     keywords = {TLS, Point cloud, Open-source, Multi-view data registration, LiDAR data metrics, Robust loss function, Tait-bryan angles, Quaternions, Rodrigues’ formula, Lie algebra, Rotation matrix parameterization},
     abstract = {This study addresses multi-view Terrestrial Laser Scanning Point Cloud data registration methods. Multiple rigid point cloud data registration is mandatory for aligning all scans into a common reference frame and it is still considered a challenge looking from a large-scale surveys point of view. The goal of this work is to support the development of cutting-edge registration methods in geoscience and mobile robotics domains. This work evaluates 3 data sets of total 20 scenes available in the literature. This paper provides a novel open-source framework for multi-view Terrestrial Laser Scanning Point Cloud data registration benchmarks. The goal was to verify experimentally which registration variant can improve the open-source data looking from the quantitative and qualitative points of view. In particular, the following scanners provided measurement data: Z+F TLS Imager 5006i, Z+F TLS Imager 5010C, Leica ScanStation C5, Leica ScanStation C10, Leica P40 and Riegl VZ-400. The benchmark shows an impact of the metric e.g. point to point, point to projection onto a plane, plane to plane etc..., rotation matrix parameterization (Tait-Bryan, quaternion, Rodrigues) and other implementation variations (e.g. multi-view Normal Distributions Transform, Pose Graph SLAM approach) onto the multi-view data registration accuracy and performance. An open-source project is created and it can be used for improving existing data sets reported in the literature, it is the added value of the presented research. The combination of metrics, rotation matrix parameterization and optimization algorithms creates hundreds of possible approaches. It is shown that chosen metric is a dominant factor in data registration. The rotation parameterization and other degrees of freedom of proposed variants are rather negligible compared with chosen metric. Most of the proposed approaches improve registered reference data provided by other researchers. Only for 2 from 20 scenes it was not possible to provide significant improvement. The largest improvements are evident for large-scale scenes. The project is available and maintained at https://github.com/MapsHD/HDMapping.}
}
```
Tested on following datasets:

![datasets](images/datasets.jpg)

Figure: Three publicly available data sets are incorporated into the benchmark.

First row: **ETH**, second row: **RESSO**, third and fourth rows: **WHU_TLS**.

```
ETH:
@article{THEILER2014149,
     title = {Keypoint-based 4-Points Congruent Sets – Automated marker-less registration of laser scans},
     author = {Pascal Willy Theiler and Jan Dirk Wegner and Konrad Schindler},
     journal = {ISPRS Journal of Photogrammetry and Remote Sensing},
     volume = {96},
     pages = {149-163},
     year = {2014},
     issn = {0924-2716},
     doi = {https://doi.org/10.1016/j.isprsjprs.2014.06.015},
     url = {https://www.sciencedirect.com/science/article/pii/S0924271614001701}
}

RESSO:
@article{chen2017plade,    
     title = {PLADE: A Plane-based Descriptor for Point Cloud Registration with Small Overlap},    
     author = {Chen, Songlin and Nan, Liangliang and Xia, Renbo and Zhao, Jibin and Wonka, Peter},    
     booktitle = {IEEE Transactions on Geoscience and Remote Sensing}, 
     volume={58},
     number={4},
     pages={2530-2540},     
     year = {2020} 
}

WHU_TLS:
@article{DONG2020327,
     title = {Registration of large-scale terrestrial laser scanner point clouds: A review and benchmark},
     author = {Zhen Dong and Fuxun Liang and Bisheng Yang and Yusheng Xu and Yufu Zang and Jianping Li and Yuan Wang and Wenxia Dai and Hongchao Fan and Juha Hyyppä and Uwe Stilla},
     journal = {ISPRS Journal of Photogrammetry and Remote Sensing},
     volume = {163},
     pages = {327-342},
     year = {2020},
     issn = {0924-2716},
     doi = {https://doi.org/10.1016/j.isprsjprs.2020.03.013},
     url = {https://www.sciencedirect.com/science/article/pii/S0924271620300836}
}
```


