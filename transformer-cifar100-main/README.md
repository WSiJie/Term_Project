# Transformer模型使用方法

使用pycharm打开CNN_Transformer项目

### Train :
```
python train.py -c configs/default.yaml --name "name_of_exp"
```

### test :
```python
python test.py -c configs/default.yaml --name "test" -p checkpoint/name_of_exp_checkpoint.pyt

```
## 参考资料:
* [Incorporating Convolution Designs into Visual Transformers](https://arxiv.org/pdf/2103.11816v2.pdf)
* https://github.com/rishikksh20/CeiT-pytorch.git
* https://github.com/weiaicunzai/pytorch-cifar100.git

# Resnet-18项目使用

### 运行方法：
在pycharm里运行cifrapytorch.py，可以在originnet3中获得log文件以及weights文件，运行visuallize.py可以获得cifar-100图片的可视化结果，结果保存在pic1文件夹。

### tensorbaord结果查看：
在pycharm的终端里输入tensorboard --logdir [项目地址]\CIFAR-100-CUTOUT-CUTMIX-MIXUP\originnet3\logs\baseline_test可以获得baseline的测试结果。其他结果类似。

 
参考资料
mixup:https://github.com/facebookresearch/mixup-cifar10
cutout:https://github.com/uoguelph-mlrg/Cutout
cutmix:https://github.com/clovaai/CutMix-PyTorch
