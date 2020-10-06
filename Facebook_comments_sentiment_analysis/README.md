## Sentiment Analysis for Facebook Data using Fully Connected Feedforward network using PyTorch
  
Training Accuracy achieved: 0.985 </br>
Validation Accuracy achieved : 0.92 </br>

The libraries imported include:

    import pandas as pd
    import numpy as np

    from sklearn.model_selection 
    import KFoldfrom sklearn.ensemble import RandomForestClassifier
    
    import torch
    import torch.nn as nn
    import torch.nn.functional as F from torch.utils.data
    import TensorDataset, DataLoader
    import torch.optim as optim

Steps in the project:

    1. Load Data
    2. Data Preprocessing
    3. Traditional Machine Learning Model: Random Forest using sklearn
    4. Fully connected feedforward Neural Network using PyTorch 
       - Using unigram and bigram TF.IDF feature set
       - Using Droptout and ADAM to avoid overfitting
