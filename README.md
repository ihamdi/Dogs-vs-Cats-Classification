# Dogs vs Cats Classification 
### Using Densenet121 model and Adam optimizer on a Jupyter Notebook

## Installation:
*Conda environment created with python 3.6.13 and ipykernel on RTX 2070 and i7-10750H

Please install pytorch and the correct cudatoolkit (https://pytorch.org/get-started/locally/) then proceed to install the rest of the dependencies using "pip install -r requirements.txt".

The code is designed to download the data directly from Kaggle and extract it. Please visit www.kaggle.com and download your API token from the Settings page 
(click on your profile picture on top left and select "Settings" from the dropdown menu). Otherwise, download and extract the data in the same folder as the notebook.


## How to Use:
After importing libraries, the code will ask you for the number of epochs, dropout rate, batch size, number of workers, learning rate, local path to download data, size of dataset used, and ration for splitting the dataset into training:validation:testing. 
Afterwards, the program will run and give a summary of each epoch as well as a graph of the training and validation loss and accuracy.

## Results:
The model quickly reaches a validation and testing accuracy of 90% (within 3 epochs). Densenet121 seems to be quite powerful for this task. Even with 20% dropout, the model accuracy passes 90% at the 3rd epoch and starts overtraining.


![Training](https://user-images.githubusercontent.com/93069949/143770982-651952d3-30db-43dc-93ec-efeca15f76fe.png)

![Validation](https://user-images.githubusercontent.com/93069949/143770984-e963d341-6639-4857-950a-ceb15eecb307.png)


### Background:
This was created purely to learn the inner workings of Python and Pytorch, therefore only the training data is utilized.

### Contact:
For any questions or feedback, please feel free to post comments or contact me at ibraheem.hamdi@mbzuai.ac.ae
