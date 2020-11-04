## Handwritten digit recognition using CNN

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
