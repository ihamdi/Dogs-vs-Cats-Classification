# Dogs vs Cats Classification 
### Using Densenet121 model and Adam optimizer on a Jupyter Notebook
<a href="https://www.anaconda.org/"><img src="https://img.shields.io/badge/conda-v4.10.3-blue.svg?logo=conda&style=for-the-badge" /></a>
<a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-v1.10.0-red.svg?logo=PyTorch&style=for-the-badge" /></a>
<a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-v3.9.7-blue.svg?logo=python&style=for-the-badge" /></a>
<a href="https://jupyter.org/try"><img src="https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter" /><a>

<p align="center">
  <img width="1000" src="https://www.purelypetsinsurance.co.uk/media/1138/dog-and-kitten-meeting.jpg">
</p>

## Installation:

1. Download files or clone Github
```
import git
git.Git("/your/directory/to/clone").clone("git:https://github.com/ihamdi/Dogs-vs-Cats-Classification.git)
```
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; or [download](https://github.com/ihamdi/Dogs-vs-Cats-Classification/archive/refs/heads/main.zip) and extract a copy of the files.

2. Create conda environment
```
conda create --name env-name ipykernel
```

3. Install [PyTorch](https://pytorch.org/get-started/locally/) according to your machine. For example:
```
conda install pytorch torchvision torchaudio cudatoolkit=10.2 -c pytorch
```

4. Install dependencies from [`requirements.txt`](https://github.com/ihamdi/Dogs-vs-Cats-Classification/blob/main/requirements.txt) file:
```
pip install -r requirements.txt
```

5. Download the data:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; The code is designed to download the data using the Kaggle API and extract it automatically. If you haven't used Kaggle API before, please look at the section at the bottom on how to download your API key.
  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Alternatively, you can download the data from the official [Dogs vs. Cats](https://www.kaggle.com/c/dogs-vs-cats/data) competition page and extract train.zip to the [`train`](https://github.com/ihamdi/Dogs-vs-Cats-Classification/tree/main/train) folder.

## How to Use:
Click Run All for the [`pytorch-cat-vs-dog.ipynb`](https://github.com/ihamdi/Dogs-vs-Cats-Classification/blob/main/pytorch-cat-vs-dog.ipynb) Jupyter Notebook. After the necessary libraries are imported, you will be asked to input the following:
1. Number of epochs
2. Dropout rate
3. Batch size
4. Number of workers
5. Learning rate
6. Local path (to download data)
7. Amount of dataset used
8. Ratio for splitting the dataset (into training : validation : testing)
 
Afterwards, the program will run, giving a summary after each epoch as well as a graph of the training and validation losses and accuracies.

## Results:
Densenet121 seems to be quite powerful for this task. Even with 20% dropout, the model accuracy passes 90% by the 3rd epoch and starts overfitting.

Training Loss & Accuracy             |  Validation Loss & Accuracy
:-------------------------:|:-------------------------:
<img width="500" src="https://user-images.githubusercontent.com/93069949/144221977-6e011636-ef82-49ba-a895-9469889556d2.jpg"> | <img width="500" src="https://user-images.githubusercontent.com/93069949/144221902-9cd6d94f-97ca-4914-a1f2-191667a3b50b.jpg">


### Background:
This was created purely to gain hands-on experience of Python and Pytorch. Only the training data is utilized and no submission is made to the competition.

---

### Contact:
For any questions or feedback, please feel free to post comments/issues or contact me at ibraheem.hamdi@mbzuai.ac.ae

---

### References:
  
[Densenet paper](https://arxiv.org/abs/1608.06993) by Gao Huang, Zhuang Liu, Laurens van der Maaten, Kilian Q. Weinberger.

[Dogs vs. Cats](https://www.kaggle.com/c/dogs-vs-cats/data) competition on [Kaggle](www.kaggle.com).
  
[[pytorch] cat vs dog](https://www.kaggle.com/jaeboklee/pytorch-cat-vs-dog) code from Kaggle was used to learn using Pytorch.

---
#### *Using Kaggle's API
![image](https://user-images.githubusercontent.com/93069949/144188576-d457568e-7cd2-42f2-ba08-9c41143d674d.png)

![image](https://user-images.githubusercontent.com/93069949/144188635-705e1e29-92ae-4aba-be66-0e1d2e1c29ca.png)

![image](https://user-images.githubusercontent.com/93069949/144188696-f535f9c8-3ed8-4e1b-8f0d-179d7e5be2a2.png)
