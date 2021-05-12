# Baseline
Baseline for [2nd Anti-UAV Challenge](https://anti-uav.github.io).

<div align="center">
  <img src="anti-uav.gif" width="600px" />
</div>

## Download Dataset

- `test-dev`:  [Google Drive](https://drive.google.com/file/d/1UCyapTkvYGJsfn21iUFInHANbDIAkSeX/view?usp=sharing) and [Baidu Yun](https://pan.baidu.com/s/11OnXAzT28WWFqaKPPy00DA)(vfjb)

- `test-challenge`: The test-challenge will be released on 3rd July.

**Note**: 

- We provide Thermal Infrared (IR) videos and their ground-truth labels. Contestants can only use the ground- truth bounding box of the target in the first frame. For a comprehensive comparison of different trackers, we evaluate them on video sequences with various challenging attributes. Our evaluation ranks are calculated according to the overall performance on all video sequences.



## Test
- set up the environment
```shell
conda create -n anti_uav python=3.7
conda activate anti_uav
pip install opencv-python torch
```
- run
```shell
python test.py
```
- You will see the following results.
  
```shell
[001/100]  20190925_131530_1_4    IR Fixed Measure: 0.187
[002/100]  20190926_183400_1_8    IR Fixed Measure: 0.788
...
[100/100]  20190925_213001_1_2    IR Fixed Measure: 0.028
[Overall]    IR Mixed Measure: 0.420
```

# Submit result to [codalab](https://competitions.codalab.org/competitions/23881)

```
cd results/SiamFC
zip -r ../SiamFC_test_challenge.zip *.txt
```

You can upload the `SiamFC_test_challenge.zip` file to codalab(https://competitions.codalab.org/competitions/23887).

