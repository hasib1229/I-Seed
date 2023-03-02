# I-Seed detection


## Training

Description:

    Train I-Seed detection an image.

Usage:

```
    $ python path/to/train.py --model_selected yolo --data ../Artificial_Seed_Chip_2.0-2/data.yaml --epochs 300 --img_size 512 --batch 16


```

Output:

    Files saved to:

      /runs/train/{exp_num}/

    This folder contains:

*    model weights

*    train logs


## Instalation

### Tested with python 3.8

```
    $ conda create --name py38 python=3.8

    $ conda activate py38

```

### install dependencies: (use cu111 because colab has CUDA 11.1)
```
    $ pip install torch==1.9.0+cu111 torchvision==0.10.0+cu111 -f https://download.pytorch.org/whl/torch_stable.html
```
### install mmcv-full thus we could use CUDA operators
```
    $ pip install mmcv-full -f https://download.openmmlab.com/mmcv/dist/cu111/torch1.9.0/index.html
```
### install other necessary modules
```
    $ pip install -r requirements.txt
```


