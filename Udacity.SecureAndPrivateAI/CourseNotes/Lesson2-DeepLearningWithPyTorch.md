## Lesson 2 - Deep Learning with PyTorch

#### Preparation
1. Clone repo:
`git clone https://github.com/udacity/deep-learning-v2-pytorch.git`

2. Go to `intro-to-pytorch`

#### Dependencies
- PyTorch v0.4
    - `conda install numpy jupyter notebook`
    - PyTorch site => stable version
    - `conda install pytorch torchvision cudatoolkit=9.0 -c pytorch`
- Miniconda, Anaconda
- May need GPU

#### Part 1- Tensors in PyTorch

```
import torch
```

```
def activation(x):
    """ Sigmoid activation function 
    
        Arguments
        ---------
        x: torch.Tensor
    """
    return 1/(1+torch.exp(-x))
```

```
### Generate some data
torch.manual_seed(7) # Set the random seed so things are predictable

# Features are 5 random normal variables (from a normal distribution with 0 mean and 1 standard deviation)
features = torch.randn((1, 5))
# True weights for our data, random normal variables again
# .randn_like(tensor) creates a tensor like another, with values from a normal distribution
weights = torch.randn_like(features)
# and a true bias term
bias = torch.randn((1, 1))
```

- `torch.sum()`
- `torch.mm()`
- `torch.matmul()`
- `tensor.reshape(a,b)`
- `tensor.resize_(a,b)`
- `tensor.view(a,b)`






