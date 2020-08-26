# NLP_Named_Entity_Recognition_System

In this project is the implementation of <strong>Named Entity Recognition System</strong> using <strong>LSTMs</strong> with Trax. 

NER is a subtask of information extraction that locates and classifies named entities in a text. The named entities could be organizations, persons, locations, times, etc.

Click [Jupyter Notebook](https://github.com/aprasad13/NLP_Named_Entity_Recognition_System/blob/master/Named_Entity_Recognition.ipynb) to access the detailed code.

## Following steps were involved:
- Explored the data and understood the meaning of various tags
    - Imported the Data
    - Created a Data generator which releases the data in batches without occupying the memory
- Build the model (Design the architecture of a neural network LSTMs)
    - Used the input tensors we built in our data generator
    - Feeded it into an Embedding layer, to produce more semantic entries
    - Feeded it into an LSTM layer
    - Run the output through a linear layer
    - Run the result through a log softmax layer to get the predicted class for each word.
- Trained the Model
    - Model = LSTM
    - Loss funtion = Cross Entropy Loss
    - Optimizer = Adam
- Computed an <strong>accuracy of 94.57 %</strong> on validation set and <strong>accuracy of 94.61 %</strong> on test set
- Tested with our own sentence
