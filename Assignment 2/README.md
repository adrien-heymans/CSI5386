# CSI5386 - Assignment 2
Repository for the class CSI5386 - Natural Language Processing

## Exercise 1

### Content 
This folder contains the code and rsults obtained for the first exercise of the assignment. 
- `/data` : Contains the training and testing data for CUAD.
- `/fine-tuning` : Containes 3 jupyter notebook, one for each model that was fine-tuned. 
- `/evaluation` : Contains the evaluation files. One file to create a `nbest_predictions.json` for each model, and another folder that contains the `evaluation.py` file (given in the provided GitHub code)
- `/trained-models` : This folder contains the checkpoints for the 3 trainined models (Bert, RoBERTA-Base and Legal BERT)

### Running the code 
To fine-tune the models, simply open the jupyter notebook in the `fine-tuning` folder, and run the cells one-by one. (You might have to change the file path in the cells, depending on where you run the code)

To test the evaluation, simply eexecute the `evaluation.py` file, it will automatically calculate the the AUPR, Precision and Recall for the 3 models. 

## Exercise 2
This folder contains the training and test data for the second exercise of this assignment.
- Note that the result files are created by the preprocessing steps.
    - Preprocessing of the data is done by running the code cell in the `ex2.ipynb` file on your local machine.
- In order to run the `ex2_colab.ipynb` file you will need to open this file in colab.
    - This file expects two folders to be present in the google drive of the user running the program.
    - These two folders should be contained in a root level folder named `Datasets`.
    - The two folders themselves should be named `Training_Data` and `Test_Data`.
    - The contents of these two folders should be the files found in `Result_Files` folder of both `Test_data` and
    `Training_Data` on your local machine. Note these files are the output of the preprocessing step.
    - The expected path of all datasets can be found in the code if these instructions are not clear.
    - Finally there will be two output files in `Datasets`: `With_Training_distiluse-base-multilingual-cased-v2` and 
      `Without_Training_distiluse-base-multilingual-cased-v2`. They give the similarity scores.
