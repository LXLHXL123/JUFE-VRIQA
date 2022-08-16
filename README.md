# Perceptual Quality Assessment of Omnidirectional Images

This repository contains the constructed omnidirectional image quality assessment database and implementations for the paper "[Perceptual Quality Assessment of Omnidirectional Images](https://aaai-2022.virtualchair.net/poster_aaai4008)", [Yuming Fang](http://sim.jxufe.cn/JDMKL/ymfang.html), Liping Huang, Jiebin Yan, Xuelin Liu, and Yang Liu, *Thirty-Sixth AAAI Conference on Artificial Intelligence*, 2022.

## VR IQA Database
The proposed omnidirectional image quality assessment database and the annotations (MOS, HMD data) can be downloaded at the [Baiduyun](https://pan.baidu.com/s/1DRDeEf3yWRKuzJ7_BT3GjA) (Password: jhsx) or [Google drive](https://drive.google.com/drive/folders/1ro9D6LOhpd-t6f_X0P5Rx5dkgF8fDJPS?usp=sharing).
+ **Catalog:**<br>
├─&nbsp;AAAI2022<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;ref        &nbsp;&nbsp;&nbsp;&nbsp;// reference omnidirectional images, 1.png~258.png<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;dis        &nbsp;&nbsp;&nbsp;&nbsp;// distorted omnidirectional images, 1_len3_bd_3.png<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;HMData.zip &nbsp;&nbsp;&nbsp;&nbsp;// head/eye movement data<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;bad<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;A<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;B<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;C<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└─&nbsp;D<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└─&nbsp;good<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;A<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;B<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;C<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└─&nbsp;D<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└─&nbsp;mos.xls    &nbsp;&nbsp;&nbsp;&nbsp;// mean opinion scores
+ **Explanation:**

## Proposed Model
TBC.


## Citation
Please cite our papers if it helps your research:
```bibtex
@inproceedings{fang2022aaai,
title={Perceptual Quality Assessment of Omnidirectional Images},
author={Fang, Yuming and Huang, Liping and Yan, Jiebin and Liu, Xuelin and Liu, Yang},
booktitle={Thirty-Sixth AAAI Conference on Artificial Intelligence},
pages={580-588},
year={2022}
}
