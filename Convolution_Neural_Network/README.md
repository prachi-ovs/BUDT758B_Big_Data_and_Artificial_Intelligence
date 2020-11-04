## Handwritten digit recognition using CNN - MNIST Dataset

The libraries imported include:

    import pandas as pd
    import numpy as np
    
    import torch
    import torch.nn as nn
    import torch.nn.functional as F from torch.utils.data
    import torch.optim as optim
    
    import os
    import glob
    import numpy as np  
    from skimage import io 
    from torch.utils.data import Dataset, DataLoader
    
    from skimage import transform
    from torchvision import transforms, utils
    from torch.utils.data import random_split
    
The MNIST dataset is used in this project but certain data customization tasks have been performed such as:

    Rescale: Rescale each instance to a 1 x 28 x 28 numpy array
    ToTensor: Convert each instance into a dictionary with 2 key-value pairs. 
              The first value is the Tensor of the instance (image) and the second value is the label of the instance as a tensor
 
