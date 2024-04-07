# TensorflowProjectLTH
### Tensorflow project about initialization of sparse networks based on extracted structural features of "winning tickets"

The experiment can be separated into 4 steps: the creation of winning tickets, the extraction of structural features from the winning tickets, the implementation of the extracted structural features in sparse networks, and testing the training performance of the modified sparse networks. These four steps are distributed onto three notebooks:  

The notebook [**"Creating Lottery Tickets.ipynb"**](https://github.com/Ernalein/TensorflowProjectLTH/blob/main/Creating%20Lottery%20Tickets.ipynb) is were the first step is attempted. The lottery tickets are created using iterative magnitude pruning, tested whether they are winning tickets, and if so, stored in files.  

[**"Extracting and implementing structural features of winning tickets.ipynb"**](https://github.com/Ernalein/TensorflowProjectLTH/blob/main/Extracting%20and%20implementing%20structural%20features%20of%20winning%20tickets.ipynb)  holds the second, third, and parts of the last step. From winning tickets, three types of structural features are extracted. Since we did not succesfully create winning tickets, we use [Hollers winning tickets](https://github.com/Ernalein/TensorflowProjectLTH/tree/main/isabels_wts) for this step. The extracted structural features are then implemented in sparse networks which are then trained. The accuracies measured during training of these networks are stored in a the file ["experiment_accuracies.npy"](https://github.com/Ernalein/TensorflowProjectLTH/blob/main/experiment_accuracies.npy).  

Lastly, [**"Significance testing.ipynb"**](https://github.com/Ernalein/TensorflowProjectLTH/blob/main/Significance%20testing.ipynb) is where the measured accuracies are used to test the hypotheses via paired samples t-tests. The formulated hypotheses are noted here as well.

