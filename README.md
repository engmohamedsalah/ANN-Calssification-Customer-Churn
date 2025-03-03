
# Customer Churn Prediction

This project is designed to predict customer churn using a machine learning model. The model is built using TensorFlow and various preprocessing techniques to handle the input data.

## Project Structure
. ├── .gitignore ├── ann-venv/ ├── app.py ├── Churn_Modelling.csv ├── experiments.ipynb ├── label_gender_encoder.pkl ├── logs/ ├── model.h5 ├── onehotencoder.pkl ├── prediction.ipynb ├── requirements.txt ├── scaling_parameters.pkl


- `app.py`: The main application file that uses Streamlit to create a web interface for predicting customer churn.
- `Churn_Modelling.csv`: The dataset used for training and testing the model.
- `experiments.ipynb`: Jupyter notebook containing the experiments and model training process.
- `label_gender_encoder.pkl`: Pickle file for the label encoder used for the gender feature.
- `logs/`: Directory containing logs.
- `model.h5`: The trained model file.
- `onehotencoder.pkl`: Pickle file for the one-hot encoder used for the geography feature.
- `prediction.ipynb`: Jupyter notebook for making predictions using the trained model.
- `requirements.txt`: List of dependencies required for the project.
- `scaling_parameters.pkl`: Pickle file for the scaler used to scale the input features.

## Setup

1. Clone the repository:
    ```sh
    git clone <repository-url>
    cd <repository-directory>
    ```

2. Create a virtual environment and activate it:
    ```sh
    python -m venv ann-venv
    source ann-venv/bin/activate  # On Windows use `ann-venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

4. Run the Streamlit app:
    ```sh
    streamlit run app.py
    ```

## Usage

1. Open the Streamlit app in your browser.
2. Enter the required input features such as Geography, Gender, Age, Balance, Credit Score, and Estimated Salary.
3. Click the "Predict" button to get the churn prediction and probability.

## Model Training

The model is trained using the data in [Churn_Modelling.csv](http://_vscodecontentref_/9). The training process is documented in [experiments.ipynb](http://_vscodecontentref_/10). The following steps are performed:

1. Data preprocessing including encoding categorical features and scaling numerical features.
2. Training a neural network using TensorFlow.
3. Saving the trained model and preprocessing objects (scalers and encoders) as pickle files.

## License

This project is licensed under the MIT License.