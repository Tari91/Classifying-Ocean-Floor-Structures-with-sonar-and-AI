# **Classifying Ocean Floor Structures with Sonar and AI**

This project demonstrates how to use synthetic sonar data and machine learning to classify different ocean floor structures such as **Sand**, **Rock**, and **Coral**. A neural network model is trained on simulated sonar data to recognize patterns associated with each type of ocean floor.

## 📦 Files

- `synthetic_sonar_ocean_floor.xlsx` — Synthetic dataset containing sonar feature data and labeled ocean floor types.
- `sonar_classification.py` — Main Python script that:
  - Generates synthetic sonar data
  - Preprocesses the data
  - Trains a neural network classifier
  - Evaluates the model
  - Visualizes results (accuracy, confusion matrix)

## 📊 Dataset

The dataset contains **2,000 samples** and **10 numerical features** generated using `sklearn.datasets.make_classification()`. The target labels represent three types of ocean floor structures:
- `Sand`
- `Rock`
- `Coral`

## 🧠 Model

A simple feedforward neural network (MLP) is implemented using **TensorFlow/Keras**. It includes:
- Input layer with ReLU activation
- Dropout for regularization
- Output layer with softmax for 3-class classification

## 🔧 Requirements

- Python 3.8+
- TensorFlow
- scikit-learn
- pandas
- matplotlib
- seaborn

Install the required libraries with:

```bash
pip install tensorflow scikit-learn pandas matplotlib seaborn
▶️ Usage
Run the training script:

bash
python sonar_classification.py
This will train the model, print evaluation metrics, and display visualizations for accuracy and confusion matrix.

📈 Example Output
Test Accuracy: ~90% (varies due to synthetic randomness)

Confusion matrix shows class-wise performance

Accuracy plot for training vs validation

📁 Output
synthetic_sonar_ocean_floor.xlsx: Exported Excel file containing features and labeled data.

🔄 Future Work
Replace synthetic data with real sonar datasets

Experiment with more complex models like CNNs or LSTMs for temporal sonar signals

Deploy as an API using Flask or FastAPI

📜 Author
 Tarinabo williamtarinabo@gmail.com
