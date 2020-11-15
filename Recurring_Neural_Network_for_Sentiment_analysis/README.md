## Text classification based on sentiment -Amazon Reviews

The libraries imported include:

    import pandas as pd
    import numpy as np
    
    import torch
    import torch.nn as nn
    import torch.nn.functional as F from torch.utils.data
    import torch.optim as optim
    
    import os
    
    from skimage import transform
    from torchvision import transforms, utils
    from torch.utils.data import random_split
    from torch.utils.data import Dataset, DataLoader
    
Tasks done in the project include:

    1. Create a dictionary: Using `TfidfVectorizer` from sklearn to generate tf-idf values for every word in each document
    2. Data preparation: Use 1000 documents where each document is represented as a vector of size equal to maximum size of document (max_doc_size) in the dataset. 
       Each word in the document vector is represented using one hot encoding using the tfidf value for word in document calculated in the previous step instead of 1.
       Each word vector size is 200. The final result is an array of 1000 x max_doc_size x 200
    3. Create the Train loader and Validation loader
    4. Create a multi-layer RNN 
    5. Traning and Validation: For each batch in training, the average validation loss for all instances in the validation set is printed.
