# 3D High-quality Garment Dataset
Official dataset for "Automatic Pose and Wrinkle Transfer for Aesthetic Garment Display" (Computer-Aided Geometric Design, 2021).

[[Project Page]](http://www.cad.zju.edu.cn/home/jin/cagd2021/cagd2021.htm) [[Paper]](https://www.sciencedirect.com/science/article/pii/S0167839621000650)

![avatar](http://www.cad.zju.edu.cn/home/jin/cagd2021/teaser.jpeg)

## Download the Dataset
The dataset can be downloaded via [Google Drive] (https://drive.google.com/file/d/14cq_Sa8hkEO3u9HZF5N7jWK2Xu92US29/view?usp=sharing).

## Dataset Description
Our dataset contains a total of 19 paired garment models in 9 types, including:
1. women's T-shirts (2)
2. women's shirts & shirts with notched sleeves (3)
3. women's casual trousers (2)
4. women's gowns (2)
5. men's sports suits (top) (2)
6. men's sports suits (bottom) (2)
7. women's Qipao & polo dress (2)
8. women's lantern sleeve dresses (2)
9. men's hoodies (2)

In the folder of each garment type, we provide files of two paired garment models (three for women's shirts) with similar styles. The file structure of the dataset is as follows:

```
ROOT/
---- garment_type_1/
-------- garment_1/
------------- garment_1_def/
------------------ garment_1_def.obj
------------------ garment_1_def_sculpted.obj

------------- garment_1_patterns/
------------------ garment_1_2D.obj

------------- garment_1_ref/
------------------ garment_1_ref.obj
------------------ garment_1_ref_smoothed.obj

-------- garment_2/
------------- garment_2_result/
------------------ garment_2_result.obj 
         
------------- garment_2_patterns/
------------------ garment_2_2D.obj
        
------------- garment_2_ref/
------------------ garment_2_ref.obj
------------------ garment_2_ref_smoothed.obj

-------- projects/
------------- garment_1_ref.Zprj
------------- garment_1_def.Zprj
------------- garment_2_ref.Zprj

---- garment_type_2
...
...
---- garment_type_9
README.md
```
- We use `garment_1` as the source and `garment_2` as the target in the experiments of our paper.
- Users may edit garment projects using [CLO](https://www.clo3d.com/). The version we use is 5.2.
- `garment_2_result.obj` is the transfer result of our method.
- In the folder `women's_shirts/`, `shirt_1` can be paired with `shirt_2` and `shirt_2_notched_sleeves` for pose and wrinkle transfer, respectively. `shirt_2_notched_sleeves` is designed for the experiment about prooving our method can handle surfaces of different topologies.


## Citation
If you use this dataset for your research, please cite our paper:

```
@article{WANG2021102020,
title = {Automatic pose and wrinkle transfer for aesthetic garment display},
journal = {Computer Aided Geometric Design},
volume = {89},
pages = {102020},
year = {2021},
issn = {0167-8396},
doi = {https://doi.org/10.1016/j.cagd.2021.102020},
url = {https://www.sciencedirect.com/science/article/pii/S0167839621000650},
author = {Luyuan Wang and Honglin Li and Qinjie Xiao and Xinran Yao and Xiaoyu Pan and Yuqing Zhang and Xiaogang Jin},
keywords = {Garment wrinkles, Deformation transfer, Aesthetic garment display, Semantic information}
}
```

## Contact
- Luyuan Wang (iriswang@zju.edu.cn)
