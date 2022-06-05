## Vision Transformer

We train LVT, CrossViT, ResNet18 in our project.

We run with pytorch 1.7.1. You should have visualizer installed. See [Link](https://github.com/luo3300612/Visualizer) for details.

Also to download the ImageNet pretrain weight for LVT and CrossViT from [here](). 

### Train Transformer

```
python train_transformer.py --model {model name} --dataaug {data augmentation} --lr {learning rate} --epoch {epoch} --batch_size {batch size} --resume {whether to load from checkpoint}
```

Models should be chosen from 'lvt_finetune', 'lvt_params', 'lvt_flops', 'crossvit'.

Data augmentation should be chosen from 'baseline', 'mixup', 'manimix', 'cutmix', 'mixtoken'.

### Train ResNet18

```
python train_res.py
```

### Visulizer

`visualize.ipynb` shows the attention map of our model. 

Our models can be download from [here]().

### Results

![image-20220605110600148](imgs\image-20220605110600148.png)

![image-20220605110634345](imgs\image-20220605110634345.png)

![image-20220605110647644](imgs\image-20220605110647644.png)

![image-20220605110727396](imgs\image-20220605110727396.png)

![image-20220605110704629](imgs\image-20220605110704629.png)