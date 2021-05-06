# tableImageParser

### 本项目通过腾讯分享文章，复现了腾讯表格结果解析文章地址为https://zhuanlan.zhihu.com/p/69793742   (Table Structure Recognition from Tencent)

## 环境(Requirements)
```sudo yum install -y geos-devel freetype-devel libpng-devel```

```pip install -r requirements.txt```

## 例子🌰(Demo)
- 修改inference 中main函数所需路径

```python inference.py```

## 训练(train)
- 修改train.py 中checkpoint_path 为模型路径
- 修改dataf.py 中training_data_path 为训练数据路径

```python train.py```

## 可视化实例
### 例子🌰1
![raw](https://github.com/tommyMessi/tableImageParser_tx/blob/master/tx_infer_data/vanke_2016_1241_nb_3.jpg)
![nrow](https://github.com/tommyMessi/tableImageParser_tx/blob/master/tx_infer_data/nrow/vanke_2016_1241_nb_3.jpg)
![ncol](https://github.com/tommyMessi/tableImageParser_tx/blob/master/tx_infer_data/ncol/vanke_2016_1241_nb_3.jpg)
### 例子🌰2
![raw](https://github.com/tommyMessi/tableImageParser_tx/blob/master/tx_infer_data/1.jpg)
![row](https://github.com/tommyMessi/tableImageParser_tx/blob/master/tx_infer_data/row/1.jpg)
![row](https://github.com/tommyMessi/tableImageParser_tx/tree/master/tx_infer_data/col)

## 更新 8.17
- 修改dataf.py 中的数据预处理，具体效果 根据自己数据进行适量修改。（数据增强对效果还很重要）
- 添加post.py 用于后处理的demo。具体思路通过霍夫变换的HoughLinesP函数的线段合集，进行直线断连接修复。
- 预训练模型： 链接: https://pan.baidu.com/s/1JXEKuWYtbyF6vFGQIzyE6g 提取码: 4mbb

## 其他
训练数据与预训练模型 关注微信公众账号 hulugeAI 留言：table parser



