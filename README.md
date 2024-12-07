**Classification and Regression Models on Multiple Datasets**
This project implements various machine learning models to classify and predict outcomes across six
datasets using Python and scikit-learn. Each script is designed to be executed in **Google Colab**.
**Contents**

- Requirements
- Setup
- How to Run
- Datasets : Dataset 1 , Dataset 2 , Dataset 3 , Dataset 4 , Dataset 5 , Dataset 6
- Results
**Requirements**
- Python 3.x
- Libraries:
o pandas
o numpy
o scikit-learn
o matplotlib

```
NOTE : Google Drive with the following file structure:
/content/drive/MyDrive/Project/Classification /
```
- ├── TrainData/
├── TrainData1.txt
├── TrainData2.txt
├── TrainData3.txt
├── TrainData4.txt
├── TrainData5.txt
├── TrainData6.txt
- ├── TrainLabel/
├── TrainLabel1.txt
├── TrainLabel2.txt
├── TrainLabel3.txt
├── TrainLabel4.txt
├── TrainLabel5.txt
├── TrainLabel6.txt
- ├── TestData/
├── TestData1.txt
├── TestData2.txt
├── TestData3.txt
├── TestData4.txt
├── TestData5.txt
├── TestData6.txt

**Setup**

1. ***** Upload the Datasets** : Place the training and test dataset files (TrainDataX.txt,
    TrainLabelX.txt, and TestDataX.txt) in the corresponding directories in your Google Drive.
2. **Install Dependencies** : Run the following command in a Colab notebook to install the required
    libraries:


3. !pip install pandas numpy scikit-learn matplotlib (all necessary modules)

***** How to Run**

1. Open Google Colab and mount your Google Drive:
2. from google.colab import drive
3. drive.mount('/content/drive')
4. Upload the script for the dataset you want to run into a Colab cell.
5. Execute the script to process the data, train models, and test the predictions.
6. The test dataset (TestDataX.txt) will be used to generate predictions, which will be saved to
    the results file **named model_predictions_datasetX.csv.**

**Datasets
Dataset 1: Classification with 5 Models
Input file:**

```
Models: Random Forest, Support Vector Machine, Logistic Regression-Nearest Neighbors
Naive Bayes
```
- **Outputs** : Model metrics (Accuracy, Precision, Recall, F1 Score),Predictions on test data saved
    as model_predictions_dataset1.csv
**Similar steps and file structure as Datasets 1 till dataset**
- Outputs: Predictions on test data saved as model_predictions_datasetx.csv x=2,3,4,
**Dataset 6: Regression with 4 Models**
- **Training Data** : TrainData6.txt, TrainLabel6.txt; **Test Data** : TestData6.txt
- **Models** : Random Forest Regressor, Support Vector Regressor, Linear Regression-Nearest
Neighbors Regressor
- **Metrics** : Mean Absolute Error (MAE), Mean Squared Error (MSE), R-squared (R²)
- **Output:** Predictions on test data saved as model_predictions_dataset6.csv

# 2) Missing value Estimation

**Output Saved** : Saves imputed datasets as .csv files for further use they are converted into txt.
**Files Processed**

**The script processes datasets stored at the following paths:**

# Input File: /content/drive/MyDrive/Project/MissingData/MissingData1.txt

# 3) Multi-Label Classifier


```
File Paths
Ensure the following files are available at the specified paths:
```
- **Training Data** : /content/drive/MyDrive/Project/MultiLabelData/MultLabelTrainData.txt
- **Training Labels** : /content/drive/MyDrive/Project/MultiLabelData/MultLabelTrainLabel.txt
- **Test Data** : /content/drive/MyDrive/Project/MultiLabelData/MultLabelTestData.txt
- **Output File** :
    /content/drive/MyDrive/Project/MultiLabelData/GangavaramMultiLableResult.txt

```
In Google Colab or your local environment, install missing libraries using:
!pip install numpy pandas scikit-learn lightgbm imblearn
```
**1)Prepare Your Environment** :
o Place the training and test datasets at the specified paths.
o Mount Google Drive if using Colab:
o **from google.colab import drive**
o **drive.mount('/content/drive')**

2. **Run the Script** : Execute the script in your Python environment. It will:
    o Load training and testing data.
    o Scale features using StandardScaler.
    o Perform custom multi-label SMOTE on the training data.
    o Train a LightGBM model with cross-validation.
    o Evaluate performance using accuracy and Hamming loss.
    o Generate predictions for the test dataset.
3. **Output** :
    o **The test predictions are saved to**
       **/content/drive/MyDrive/Project/MultiLabelData/GangavaramMultiLableResult.txt**


