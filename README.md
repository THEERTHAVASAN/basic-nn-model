Developing a Neural Network Regression Model

AIM :

    To develop a neural network regression model for the given dataset
    
STEPS

STEP 1:

      Loading the dataset

STEP 2:

      Split the dataset into training and testing

STEP 3:

      Create MinMaxScalar objects ,fit the model and transform the data.

STEP 4:

      Build the Neural Network Model and compile the model.

STEP 5:

      Train the model with the training data.

STEP 6:

      Plot the performance plot

STEP 7:

      Evaluate the model with the testing data.

PROGRAM
rom google.colab import auth
import gspread
from google.auth import default
import pandas as pd
auth.authenticate_user()
creds, _ = default()
gc = gspread.authorize(creds)
worksheet = gc.open('myfrenz').sheet1
rows = worksheet.get_all_values()
df = pd.DataFrame(rows[1:], columns=rows[0])
df = df.astype({'regno':'float'})

Output:
        recent:///159a3a683eaa323f7b3f0654632ef38f

RESULT:
A neural network regression model for the given dataset is verified


