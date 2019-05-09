# Tutorial for tensorflow image classification 

Different  image processing techniques with deep learning:

![Alt text](img_info/id1.png)

## Requirements
Windows 
Anaconda installation:  https://www.anaconda.com/distribution/  

## Prepare the environment
In a CMD write following commands

```
conda create -n train_class python=3.6
```

```
activate train_class
```

( move to the directory where you want your project i.e.  cd D:\CIAT\Cenicana_train\)

```
mkdir kagle
```

## Download dataset
https://www.kaggle.com/c/aerial-cactus-identification/data

unzip the dataset and train and test folders in kaggle dir
Then two folders into kaggle dir, train and test and a file train.csv

## Install tensorflow

In CMD write

```
pip install tensorflow==2.0.0-alpha0 
```

```
Jupyter lab
```
Then Jupyter lab will open and you will find training.ipynb file there , open it and run the first cell to check if the kernel is ok
```
import sys 
sys.executable
```
Output: 'C:\\Users\\jvergara\\.conda\\envs\\train_class\\python.exe'

If the output have the python.exe inside envs folder , kernel is ok  if not follow next steps:

In CMD write (Change env_name for your environment name)
```
conda install ipykernel (type “y” when prompted)
```
```
python -m ipykernel install --user --name env_name --display-name "Python (env_name)") 
```
To activate the kernel in jupyter lab, write in CMD

```
Jupyter lab
```

Go to Kernel tab and select change kernel, then click "Python (env_name)", test again the first cell 

## dependencies 
To know if tensorflow and all dependencies are ok , run second cell 
```
import tensorflow as tf
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split
from IPython.display import Image, display

print(tf.__version__)
```
If it runs without errors and the ouput is  2.0.0-alpha0, you are ready to start.
