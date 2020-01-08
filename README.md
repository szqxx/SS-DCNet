# SS-DCNet
This is the repository for S-DCNet, presented in our paper:

[**From Open Set to Closed Set: Counting Objects by Spatial Divide-and-Conquer**](https://arxiv.org/abs/2001.01886)

[Haipeng Xiong](https://scholar.google.com/citations?user=AEW8GxcAAAAJ&hl=zh-CN)<sup>1</sup>, [Hao Lu](https://sites.google.com/site/poppinace/)<sup>2</sup>, Chengxin Liu<sup>1</sup>,
Liang Liu<sup>1</sup>, Zhiguo Cao<sup>1</sup>, [Chunhua Shen](http://cs.adelaide.edu.au/~chhshen/)<sup>2</sup>

<sup>1</sup>Huazhong University of Science and Technology, China

<sup>2</sup>The University of Adelaide, Australia

## Environment
Please install required packages according to `requirements.txt`.

## Data
Testing data for ShanghaiTech and UCF-QNRF dataset have been preprocessed. You can download the processed dataset from:

ShanghaiTech PartA [[Baidu Yun]]() with code: or [[Google Drive]]()

ShanghaiTech PartB [[Baidu Yun]]() with code: or [[Google Drive]]()

UCF-QNRF [[Baidu Yun]]() with code: or [[Google Drive]]()

## Model
Pretrained weights can be downloaded from:

ShanghaiTech PartA [[Baidu Yun]]() with code: or [[Google Drive]]()

ShanghaiTech PartB [[Baidu Yun]]() with code: or [[Google Drive]]()

UCF-QNRF [[Baidu Yun]]() with code: or [[Google Drive]]()

## A Quick Demo
1. Download the code, data and model.

2. Organize them into one folder. The final path structure looks like this:
```
-->The whole project
    -->data
        -->SH_partA
        -->SH_partB
        -->UCF-QNRF_ECCV18
    -->model
        -->SHA
        -->SHB
        -->QNRF
    -->Network
        -->base_Network_module.py
        -->merge_func.py
        -->class_func.py
        -->SSDCNet.py
    -->all_main.py
    -->main_process.py
    -->Val.py
    -->load_data_V2.py
    -->IOtools.py
```

3. Run the following code to reproduce our results. The MAE will be SHA: 55.571, SHB: 6.645 and QNRF: 81.864 . Have fun:)
    
       python all_main.py --dataset SHA for ShanghaiTech PartA
       
       python all_main.py --dataset SHB for ShanghaiTech PartB
       
       python all_main.py --dataset QNRF for UCF-QNRF
       


## References
If you find this work or code useful for your research, please cite:
```
@misc{xiong2020open,
    title={From Open Set to Closed Set: Supervised Spatial Divide-and-Conquer for Object Counting},
    author={Haipeng Xiong and Hao Lu and Chengxin Liu and Liang Liu and Chunhua Shen and Zhiguo Cao},
    year={2020},
    eprint={2001.01886},
    archivePrefix={arXiv},
    primaryClass={cs.CV}
}
```
