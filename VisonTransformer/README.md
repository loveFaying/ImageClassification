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
parser.add_argument('--weights', type=str, default='./jx_vit_base_patch16_224_in21k.pth',
help='initial weights path')
```
- jx_vit_base_patch16_224_in21k 下载链接
```
https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-vitjx/jx_vit_base_patch16_224_in21k-e5005f0a.pth
```

jx_vit_base_patch16_224_in21k-e5005f0a.pth 重命名为jx_vit_base_patch16_224_in21k.pth