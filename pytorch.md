# Install pytorch

## command by command
  1. conda create -n torch python=3.7 
  2. conda activate torch
  3. conda install pytorch torchvision torchaudio pytorch-cuda=11.6 -c pytorch -c nvidia
  4. conda install -c conda-forge jupyterlab 
  5. conda install matplotlib

## by script
```bash   
export CONDA_ALWAYS_YES="true"
# confirm all following "conda" commands

conda create -n torch python=3.7 
conda activate torch
conda install pytorch torchvision torchaudio pytorch-cuda=11.6 -c pytorch -c nvidia 
conda install -c conda-forge jupyterlab
conda install matplotlib

# Disable yes to all
unset CONDA_ALWAYS_YES  
```

## verification
```python
import torch
x = torch.rand(5, 3)
print(x)
```
  
