# Baseline
Baseline for [1st Anti-UAV Challenge](https://anti-uav.github.io)

## Download Dataset `test-dev`
- Google Drive
- [Baidu Yun](https://pan.baidu.com/s/14iYLSR3sfZeAbRwDyqCs-g)(p29w)

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
[001/100] 20190925_131530_1_4 Fixed Measure: 0.789
[002/100] 20190926_183400_1_8 Fixed Measure: 0.754
...
[100/100] 20190925_213001_1_2 Fixed Measure: 0.030
[Overall] Mixed Measure: 0.381
```
