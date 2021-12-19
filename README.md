# MISSFormer
Code for paper "MISSFormer: An Effective Medical Image Segmentation Transformer". Please read our preprint at the following link: [paper_address](https://arxiv.org/abs/2109.07162).

## 1. Environment

- Please prepare an environment with Ubuntu 20.04, with Python 3.6.13, PyTorch 1.8.0, and CUDA 11.1.1.

## 2. Train/Test

- Train

```bash
python train.py --dataset Synapse --root_path your DATA_DIR --max_epochs 400 --output_dir your OUT_DIR  --img_size 224 --base_lr 0.05 --batch_size 24
```

- Test 

```bash
python test.py --dataset Synapse --is_savenii --volume_path your DATA_DIR --output_dir your OUT_DIR --max_epoch 400 --base_lr 0.05 --img_size 224 --batch_size 24
```

## References
* [TransUnet](https://github.com/Beckschen/TransUNet)
* [Swin-Unet](https://github.com/HuCaoFighting/Swin-Unet)

```bibtex
@article{huang2021missformer,
  title={MISSFormer: An Effective Medical Image Segmentation Transformer},
  author={Huang, Xiaohong and Deng, Zhifang and Li, Dandan and Yuan, Xueguang},
  journal={arXiv preprint arXiv:2109.07162},
  year={2021}
}
```