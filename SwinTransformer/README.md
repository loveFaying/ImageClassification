### dataset

- 下载地址

```
http://download.tensorflow.org/example_images/flower_photos.tgz
```

- 文件目录

```
weights
	model-0.pth
	...
	model-9.pth
flower_photos 
	daisy
		*.jpg
	dandelion
		*.jpg
	roses
		*.jpg
	sunflowers
		*.jpg
	tulips
		*.jpg
```

- 图片数量

```
3671 images were found in the dataset.
2939 images for training.
732 images for validation.
```
### 环境
```
pip install -r requirements.txt
```
### train
```
python train.py
```
### predict tulip.jpg
```
python predict.py
```
### 预训练模型
- 预训练权重路径，如果不想载入就设置为空字符
```
parser.add_argument('--weights', type=str, default='./swin_tiny_patch4_window7_224.pth',help='initial weights path')
```
- swin_tiny_patch4_window7_224.pth 下载链接
```
https://github.com/SwinTransformer/storage/releases/download/v1.0.0/swin_tiny_patch4_window7_224.pth
```