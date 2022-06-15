# 任务2(Faster R-CNN不同训练方案对比)

**准备工作**

运行`voc_annotation.py`

**方案a：随机初始化训练VOC**

在`train.py`中，设置/修改参数为：

```python
pretrained = False
backbone_maskRcnn = False
Freeze_Train = False
```

**方案b：ImageNet预训练backbone网络**

在`train.py`中，设置/修改参数为：

```python
pretrained = True
backbone_maskRcnn = False
Freeze_Train = True
```

**方案c：使用coco训练的Mask R-CNN的backbone网络参数**

在`train.py`中，设置/修改参数为：

```python
pretrained = True
backbone_maskRcnn = True
Freeze_Train = True
```

**计算mAP**

先将`frcnn.py`中的`"model_path"`参数取值调整为需要读取的权重文件

再运行`get_map.py`

## Reference
https://github.com/bubbliiiing/faster-rcnn-pytorch

