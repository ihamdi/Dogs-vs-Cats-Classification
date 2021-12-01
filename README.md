# Dogs vs Cats Classification 
### Using Densenet121 model and Adam optimizer on a Jupyter Notebook
<a href="https://www.anaconda.org/"><img src="https://img.shields.io/badge/conda-v4.10.3-blue.svg?logo=conda&style=for-the-badge" /></a>
<a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-v1.10.0-red.svg?logo=PyTorch&style=for-the-badge" /></a>
<a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-v3.9.7-blue.svg?logo=python&style=for-the-badge" /></a>

<p align="center">
  <img width="1000" src="https://www.purelypetsinsurance.co.uk/media/1138/dog-and-kitten-meeting.jpg">
</p>



## Installation:

1. Download files or clone Github
```
import git
git.Git("/your/directory/to/clone").clone("git:https://github.com/ihamdi/Dogs-vs-Cats-Classification.git)
```


2. Create conda environment
```
conda create --name DogsVsCats ipykernel
```

3. Install [PyTorch](https://pytorch.org/get-started/locally/)


4. Install dependencies:
```
pip install -r requirements.txt
```

5. Download the data:

The code is designed to download the data directly using the Kaggle API and extract it automatically. If you haven't used Kaggle API before, please look at the section at the bottom on how to download your API key.

## How to Use:
After importing libraries, you will be asked to input the following:
1. Number of epochs
2. Dropout rate
3. Batch size
4. Number of workers
5. Learning rate
6. Local path (to download data)
7. Amount of dataset used
8. Ratio for splitting the dataset (into training : validation : testing)
 
Afterwards, the program will run, giving a summary after epoch as well as a graph of the training and validation losses and accuracies.

## Results:
Densenet121 seems to be quite powerful for this task. Even with 20% dropout, the model accuracy passes 90% by the 3rd epoch and starts overtraining.

Training Loss & Accuracy             |  Validation Loss & Accuracy
:-------------------------:|:-------------------------:
![1e6f48393e17_03](https://user-images.githubusercontent.com/93069949/143770982-651952d3-30db-43dc-93ec-efeca15f76fe.png) | ![1e6f48393e17_03_mask](https://user-images.githubusercontent.com/93069949/143770984-e963d341-6639-4857-950a-ceb15eecb307.png)

### Background:
This was created purely to learn the inner workings of Python and Pytorch, therefore only the training data is utilized.

---

### Contact:
For any questions or feedback, please feel free to post comments or contact me at ibraheem.hamdi@mbzuai.ac.ae

---

### References:

[Densenet paper](https://arxiv.org/abs/1608.06993) by Gao Huang, Zhuang Liu, Laurens van der Maaten, Kilian Q. Weinberger.

[[pytorch] cat vs dog](https://www.kaggle.com/jaeboklee/pytorch-cat-vs-dog) code from Kaggle was used to learn using Pytorch.

---
#### *Using Kaggle's API
![image](https://user-images.githubusercontent.com/93069949/144188576-d457568e-7cd2-42f2-ba08-9c41143d674d.png)

![image](https://user-images.githubusercontent.com/93069949/144188635-705e1e29-92ae-4aba-be66-0e1d2e1c29ca.png)

![image](https://user-images.githubusercontent.com/93069949/144188696-f535f9c8-3ed8-4e1b-8f0d-179d7e5be2a2.png)
