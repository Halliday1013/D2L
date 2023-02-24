1.返回一个符合均值为0，方差为1的[正态分布](https://so.csdn.net/so/search?q=正态分布&spm=1001.2101.3001.7020)（标准正态分布）中填充随机数的张量

> torch.randn(*size, *, out=None, dtype=None, layout=torch.strided, 
> device=None, requires_grad=False) → Tensor

```
features = torch.randn(num_examples, num_inputs,dtype=torch.float32)
```



2.numpy.random.normal(loc=0,scale=1e-2,size=shape) ，意义如下： 

1. 参数loc(float)：正态分布的均值，对应着这个分布的中心。loc=0说明这一个以Y轴为对称轴的正态分布，
2. 参数scale(float)：正态分布的标准差，对应分布的宽度，scale越大，正态分布的曲线越矮胖，scale越小，曲线越高瘦。
3. 参数size(int 或者整数元组)：输出的值赋在shape里，默认为None。

```
labels += torch.tensor(np.random.normal(0, 0.01, size=labels.size()),
                       dtype=torch.float32)
```



3.plt.rcParams()   	设置图片属性



4.plt.show()     	展示图片