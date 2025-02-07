## [torch 参数更多 ]torch.greater

### [torch.greater](https://pytorch.org/docs/stable/generated/torch.greater.html?highlight=torch+greater#torch.greater)

```python
torch.greater(input, other, *, out=None)
```

### [paddle.full](https://www.paddlepaddle.org.cn/documentation/docs/zh/api/paddle/greater_than_cn.html)

```python
paddle.greater_than(x, y, name=None)
```

其中 Pytorch 相比 Paddle 支持更多其他参数，具体如下：
### 参数映射
| PyTorch       | PaddlePaddle | 备注                                                   |
| ------------- | ------------ | ------------------------------------------------------ |
| input  | x       | 输入 Tensor，支持的数据类型包括 bool、float32、float64、int32、int64。 |
| other  |  y  |  输入 Tensor，支持的数据类型包括 bool、float32、float64、int32、int64。  |
| out | -  | 表示输出的 Tensor ， Paddle 无此参数，需要进行转写。    |


### 转写示例
#### out：指定输出
```python
# Pytorch 写法
torch.greater([3, 5], 1., out=y)

# Paddle 写法
y = paddle.greater_than([3, 5], 1.)
```
