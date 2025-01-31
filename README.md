# CDCIT
This is the source code of [**Conditional Diffusion Models Based Conditional Independence Testing**](https://arxiv.org/abs/2412.11744) (CDCIT) acceepted by AAAI 2025. Our algorithm can test the conditional independence between random variable $X$, $Y$ given $Z$, i.e.:  

$H_0: X ⫫ Y|Z  \text{ \quad v.s. \quad }  H_1:X \not ⫫ Y|Z$  

which is an important problem in statistics, machine learning and causal structure learning. The random variables $X, Y, Z$ can represent gene expression levels, a characterization of a particular disease, or clinical information. And they may also be high-dimensional random variables. We utilize [Diffusion Models](https://arxiv.org/abs/2011.13456) and the [Conditional Randomization Test (CRT)](https://arxiv.org/abs/2304.04183) to test the conditional independence relationships.


## Environment Requirements
numpy==1.23.5  
pandas==2.2.0  
random  
torch==1.13.1+cu117  
math  
datetime  
scipy==1.10.0  
xgboost==1.7.5  
scikit-learn==1.4.0  
warnings  
os  
copy  
matplotlib==3.7.0  
tqdm  

## Usage
There is detailed description of function **perform_diffusion_crt()** in diffusion_crt.py. Show_case.ipynb also provides the usage.
