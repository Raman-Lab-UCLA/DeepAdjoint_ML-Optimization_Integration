# ML-Optimization_Integration

## Requirements
The following software is required to run the provided scripts. As of this writing, the versions below have been tested and verified.

-Python 3.7

-Pytorch 1.9.0

-scikit-image 0.18.1

Installation instructions for Pytorch (with CUDA) are at: https://pytorch.org/. For convenience, here are installation commands for the Conda distribution (after installing Anaconda: https://www.anaconda.com/products/individual).

```
conda create -n myenv python=3.7
conda activate myenv
conda install pytorch torchvision torchaudio cudatoolkit=10.2 -c pytorch
conda install -c anaconda scikit-image
```
