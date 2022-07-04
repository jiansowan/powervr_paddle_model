[简体中文](README_cn.md) | English

# powervr_paddle_model

## Introduction
This is an Imagination NCSDK enabled PaddlePaddle model zoo. The source model is from PadlePaddle model zoo. Utilize Imagination NCSDK, PaddlePaddle models could be compiled and deployed on device embedded with Imagination computing IPs, such as NNA and GPU.


## System Overview


## Imagination SW and HW
HW: Unisoc ROC1
SW: NCSDK 2.8, NNA DDK 3.4, GPU DDK 1.17

## Download models
sftp server: transfer.imgtec.com
http client: https://transfer.imgtec.com
user_name:imgchinalab_public
password: public


## Running evaluation and inference
### Setup
#### Inference board
Install NNA, GPU DDK
Install NCSDK TVM Runtime
Configure and run innference server
The compiled model

#### Evaluation machine
Clone this repo

### Evaluatin
Set mode to 'Eval'
Run run_test_egret.sh

### Inference
Set mode to 'Infer'
Run run_test_egret.sh

## Performance
### Image Classification



| Model | top-1 | top-5 | time(ms)<br>bs=1 | time(ms)<br>bs=4 | Download<br>Adress |
|:----:|:----:|:----:|:----:|:----:|:----:|
|EfficientNetB0<br>(d16-w16-b16)|75.4|93.2|null|null|[link](sftp://transfer.imgtec.com/paddle_models/EfficientNetB0-AX2185-d16w16b16-ncsdk-2_8_deploy.tar.bz2)|
|EfficientNetB0<br>(non-quant)|75.9|93.7|null|null|[link](https://paddle-imagenet-models-name.bj.bcebos.com/dygraph/inference/EfficientNetB0_infer.tar)|
|EfficientNetB0<br>(d8-w8-b16)|null|null|null|null|[link](sftp://transfer.imgtec.com/paddle_models/EfficientNetB0-AX2185-d8w8b16-ncsdk-2_8_deploy.tar.bz2)|

## Contribution
Contributions are highly welcomed and we would really appreciate your feedback!!
