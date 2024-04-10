# HCLR-Net

This repository contains the PyTorch implementation for training and testing HCLR-Net, a model designed for underwater image enhancement. If you find this code useful, please consider citing our paper and starring this repository.

## Requirements

- PyTorch 1.9.0
- Python 3.8
- CUDA 11.1
- `pip install pytorch_lightning`
- Download '/core' from [Eval Repository](https://github.com/Hikari0608/Eval/tree/4bc231309262d9aba9aa6b811ef267f9cc702633)

## Training

1. Download the code.
2. Run `python train.py`.
3. Checkpoints can be found in the `./tb_logs/UCR/version_0/checkpoints` directory.

Training data:
- Input images are located in the `./Datasets/train/input` folder.
- Ground truth images are located in the `./Datasets/train/gt` folder.

Validation data:
- Input images are located in the `./Datasets/val/input` folder.
- Ground truth images are located in the `./Datasets/val/input` folder.

## Testing

1. Download and unzip the code.
2. Place your testing images in the `test_images` folder.
3. Run `python test.py`.

## Benchmark

1. Clone the evaluation repository using `git clone https://github.com/Hikari0608/Eval`.
2. Checkout to the specific commit using `git checkout 4bc231309262d9aba9aa6b811ef267f9cc702633`.
3. Set up your dataloader in `val.py`.
4. Run `bash eval.sh`.

For your convenience, we provide all paired training data and testing data used in our paper. You can download the pre-trained weights from the following link:
- [Pre-trained weights](https://pan.baidu.com/s/1qXvulXUTleu2K2aRicrzLQ)
  - Password: qe5d

Please feel free to reach out if you encounter any issues or have any questions regarding the usage of our code. We hope this repository proves helpful for your research and applications in underwater image enhancement.
