# ML-Optimization Integration (DeepAdjoint)

## Requirements
The following software is required to run the provided scripts. As of this writing, the versions below have been tested and verified.

-Python 3.6.8

-Pytorch 1.9.0


Installation instructions for Pytorch (with CUDA) are at: https://pytorch.org/. For convenience, here are installation commands for the Conda distribution (after installing Anaconda: https://www.anaconda.com/products/individual).

```
conda create -n myenv python=3.6.8
conda activate myenv
conda install pytorch torchvision torchaudio cudatoolkit=10.2 -c pytorch
conda install -c anaconda opencv
conda install -c anaconda scipy
conda install matplotlib
conda install pandas
conda install spyder
```

## Running App in MATLAB
# Prerequisites
If running Lumerical 2020_R2 and the Integration tool in MATLAB:
1) Before launching MATLAB set the path in powershell/cmd: PATH=C:\Program Files\Lumerical\v202\bin;%PATH%
2) Then launch matlab from cmd (will not work if not launched from cmd): matlab

Reference: https://support.lumerical.com/hc/en-us/articles/360034407914-appopen

# Steps
1) Run 'ML_Opt.mlapp' in MATLAB AppDesigner.
2) Update 'Path' environment variable to '...\myenv\Library\bin' directory. Ex: 'C:\Users\cyyeu\anaconda3\envs\myenv\Library\bin'
3) Set Preferences:

3.1) Path to python executable with above modules installed. Spaces between slashes need to be wrapped with double-quotes. Ex: 'C:/Users/cyyeu/anaconda3/envs/myenv/python'

3.2) Path to working directory with downloaded Lumerical files. Spaces between slashes need to be wrapped with double-quotes. Ex: 'C:/Users/cyyeu/Documents/ML-Optimization_Integration'

3.3) Path to Lumerical MATLAB api directory. Ex. 'C:/Program Files/Lumerical/v202/api/matlab'

4) Use a GAN file for integration with DeepAdjoint. You can train your own GAN using the following repo: https://github.com/Raman-Lab-UCLA/Multiclass_Metasurface_InverseDesign, or download our trained GAN here: https://drive.google.com/drive/folders/1VWaH6JUx36FPzz7rm_nU2_vWC15xoDD6?usp=sharing

5) Follow demo here:

https://user-images.githubusercontent.com/36492956/211403747-ee368d9c-6fd2-42c8-bd60-b67dfbe6a083.mp4
