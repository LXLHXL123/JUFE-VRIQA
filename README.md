# Perceptual Quality Assessment of Omnidirectional Images

This repository contains the constructed omnidirectional image quality assessment database and implementations for the paper "[Perceptual Quality Assessment of Omnidirectional Images](https://aaai-2022.virtualchair.net/poster_aaai4008)", [Yuming Fang](http://sim.jxufe.cn/JDMKL/ymfang.html), Liping Huang, Jiebin Yan, Xuelin Liu, and Yang Liu, *Thirty-Sixth AAAI Conference on Artificial Intelligence*, 2022.

## VR IQA Database
The proposed omnidirectional image quality assessment database and the annotations (MOS, HMD data) can be downloaded at the [Baiduyun](https://pan.baidu.com/s/1DRDeEf3yWRKuzJ7_BT3GjA) (Password: jhsx) or [Google drive](https://drive.google.com/drive/folders/1ro9D6LOhpd-t6f_X0P5Rx5dkgF8fDJPS?usp=sharing).
+ **Catalog:**<br>
├─&nbsp;AAAI2022<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;ref        &nbsp;&nbsp;&nbsp;&nbsp;// reference omnidirectional images, 1.png~258.png<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;dis        &nbsp;&nbsp;&nbsp;&nbsp;// distorted omnidirectional images, 1_len3_bd_3.png<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;HMData.zip &nbsp;&nbsp;&nbsp;&nbsp;// head/eye movement data<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;bad &nbsp;&nbsp;&nbsp;// group<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;A &nbsp;&nbsp;&nbsp;// session<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;B &nbsp;&nbsp;&nbsp;// session<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;C &nbsp;&nbsp;&nbsp;// session<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└─&nbsp;D &nbsp;&nbsp;&nbsp;// session<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└─&nbsp;good &nbsp;&nbsp;&nbsp;// group<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;A &nbsp;&nbsp;&nbsp;// session<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;B &nbsp;&nbsp;&nbsp;// session<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;├─&nbsp;C &nbsp;&nbsp;&nbsp;// session<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└─&nbsp;D &nbsp;&nbsp;&nbsp;// session<br>
│&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;└─&nbsp;mos.xls    &nbsp;&nbsp;&nbsp;&nbsp;// mean opinion scores
+ **Explanation:**<br>
&nbsp; 1. ref: 258 reference omnidirectional images <br>
&nbsp; 2. dis: 1032 distorted omnidirectional images <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — Nameing rule: No.reference_No.lens_Dist-type_No.level.png<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — Distortion type: bd: brightness discontinuity, gb: gaussian blur, gn: gaussian noise, st: stitching<br> 
&nbsp; 3. HMData: head/eye movement data of subjects, including two groups(bad/good start point) and four sessions in each group, each session contains data from 15 subjects.<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — bad<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — A: 1,2,...,15<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — B: 1,2,...,15<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — C: 1,2,...,15<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — D: 1,2,...,15<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — good<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — A: 1,2,...,15<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — B: 1,2,...,15<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — C: 1,2,...,15<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — D: 1,2,...,15<br>
&nbsp;&nbsp;&nbsp; Data format: csv <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — Head movement data<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; A col: pitch<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; B col: yaw<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; C col: roll<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; — Eye movement data<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; D col: latitude<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; E col: longitude<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; F col: the eye fixation is valid (1) or invalid (0)<br>
&nbsp; 4. mos.xls: mean opinion scores<br>
<table align="center">
  <tr><th align="center">session</th><th align="center">imgName</th><th align="center">average</th><th align="center">std</th><th align="center">distortionType</th><th align="center">level</th><th align="center">explorationTime</th><th align="center">startingPoint</th><th align="center">Scene</th></tr>
  <tr align="center"><td>C_good</td><td>1_len3_bd_3.png</td><td>3.533</td><td>0.499</td><td>BD</td><td>3</td><td>5s</td><td>1</td><td>CreativePark</td></tr>
  <tr align="center"><td>···</td><td>···</td><td>···</td><td>···</td><td>···</td><td>···</td><td>···</td><td>···</td><td>···</td></tr>
</table>

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
