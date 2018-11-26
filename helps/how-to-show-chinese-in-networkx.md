## 问题描述

大家好，我们在用 networkx 显示中文的时候，会发现不能显示中文。 

## 解决办法

1. [下载字体SimHei](https://www.wfonts.com/font/simhei), 该字体能够支持中文； 
2. 在 jupyter notebook 中执行
```python
import matplotlib
print(matplotlib. matplotlib.__path__)
```
找到 matplotlib 的路径，然后 cd 到这个路径。 cd 到这个路径之后，继续 cd，cd 到 mpl-data/fonts/ttf 这个路径。 然后把 `DejaVuSans.ttf` 这个文件换成我们刚刚下在的文件。 

```bash
$ mv SimHei.ttf DejaVuSans.ttf
```

