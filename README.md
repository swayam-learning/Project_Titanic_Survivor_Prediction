# Decision Tree Classifier Streamlit App

This project is a **Streamlit web application** that uses a **Decision Tree Classifier** to make predictions based on user-provided inputs. The app leverages a pre-trained machine learning model pipeline for data preprocessing and predictions, all presented through an intuitive web interface.

---

## Features

- **Pre-Trained ML Pipeline**:
  - Handles missing data imputation, one-hot encoding, feature scaling, and feature selection.
  - Uses a Decision Tree Classifier for predictions.

- **Interactive Web Interface**:
  - Input features using sliders, dropdowns, and number inputs.
  - Displays user inputs and predictions dynamically.

- **Model Flexibility**:
  - Loads a pre-trained model (`model.pkl`) by default.
  - Allows users to upload a custom `.pkl` model if the default is missing.

---

## Technologies Used

- **Python**: Programming language for the application.
- **Streamlit**: Framework for building the interactive user interface.
- **scikit-learn**: Library for creating the ML pipeline and classifier.
- **pandas**: For handling input data and preprocessing.

---

## Installation

Follow these steps to set up and run the app locally:

### 1. Clone the Repository
bash
git clone https://github.com/swayam-learning/Project_Titanic_Survivor_Prediction
### 2. Install Dependencies
Set up a virtual environment (recommended):

Copy code
python -m venv env
source env/bin/activate  # Windows: .\env\Scripts\activate
Install the required Python libraries:

Copy code
pip install -r requirements.txt
### 3. Add the Pickled Model
Ensure the pickled model pipeline (model.pkl) is in the root directory. The model must match the pipeline structure shown in the project.

### 4. Run the App
Start the Streamlit app using:

Copy code
streamlit run streamlit_decision_tree.py

### 5. Access the App
Open your browser and navigate to:
http://localhost:8501
File Structure

- ├── streamlit_decision_tree.py  # Main Streamlit app script
- ├── model.pkl                   # Pre-trained pipeline model (local file)
- ├── requirements.txt            # Python dependencies
- ├── README.md                   # Project documentation
Usage
Provide Input Features:

Enter values for features such as Pclass, Sex, Age, etc., using the web interface.
The input data will be displayed dynamically for verification.
Get Predictions:

Click the Predict button to get predictions from the model.
Upload Custom Model:

If the default model is missing or a different model is preferred, upload a .pkl file through the interface.
Input Features
- **Feature	Description**
  - Pclass	Passenger Class (1, 2, or 3)
  - Sex	Gender (male or female)
  - Age	Age of the passenger (0 - 100)
  - SibSp	Number of siblings or spouses aboard
  - Parch	Number of parents or children aboard
  - Fare	Ticket fare paid
  - Embarked	Port of Embarkation (C, Q, or S)
- **Example Input**
An example input could look like this:
  - Pclass: 3
  - Sex: male
  - Age: 29
  - SibSp: 0
  - Parch: 0
  - Fare: 7.25
  - Embarked: S
### Customization
Modify streamlit_decision_tree.py to adjust input feature types or additional functionality.
Replace the model pipeline (model.pkl) to try different models or configurations.
### Troubleshooting
  -Model Not Found:
    Ensure model.pkl exists in the project directory or upload a .pkl file through the app.
  -Prediction Errors:
    Verify that input features match the model’s training data format.

### Future Enhancements
Visualize feature importance or decision tree structure.
Add support for additional machine learning models.
Implement model retraining directly from the app.

### Additionally Hosted on Streamlit Cloud
https://titanic-survival-prediction-using-pipelining.streamlit.app/

