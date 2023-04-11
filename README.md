### requirement.txt
```
torch==2.0.0
torchvision==0.15.1
imageio==2.27.0
natsort==8.3.1
scipy==1.8
scikit-image==0.20.0
pillow==9.5.0
pandas==2.0.0
dominate==2.7.0
opencv-python==4.7.0.72
visdom==0.2.4
IPython==8.12.0

```
### model/networks/block_extractor/setup.py
```
cxx_args = ['-std=c++14']

nvcc_args = [
    #'-gencode', 'arch=compute_50,code=sm_50',
    #'-gencode', 'arch=compute_52,code=sm_52',
    '-gencode', 'arch=compute_60,code=sm_60',
    '-gencode', 'arch=compute_61,code=sm_61',
    '-gencode', 'arch=compute_70,code=sm_70',
    '-gencode', 'arch=compute_70,code=compute_70',
    '-gencode', 'arch=compute_75,code=sm_75'
]
```
### model/networks/local_attn_reshape/setup.py
```
cxx_args = ['-std=c++14']

nvcc_args = [
    #'-gencode', 'arch=compute_50,code=sm_50',
    #'-gencode', 'arch=compute_52,code=sm_52',
    '-gencode', 'arch=compute_60,code=sm_60',
    '-gencode', 'arch=compute_61,code=sm_61',
    '-gencode', 'arch=compute_70,code=sm_70',
    '-gencode', 'arch=compute_70,code=compute_70',
    '-gencode', 'arch=compute_75,code=sm_75'
]
```
### model/networks/resample2d_package/setup.py
```
cxx_args = ['-std=c++14']

nvcc_args = [
    #'-gencode', 'arch=compute_50,code=sm_50',
    #'-gencode', 'arch=compute_52,code=sm_52',
    '-gencode', 'arch=compute_60,code=sm_60',
    '-gencode', 'arch=compute_61,code=sm_61',
    '-gencode', 'arch=compute_70,code=sm_70',
    '-gencode', 'arch=compute_70,code=compute_70',
    '-gencode', 'arch=compute_75,code=sm_75'
]
```
