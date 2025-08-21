# Laptop Price Predictor

## Overview
This project implements a machine learning model to predict laptop prices based on their specifications. The model uses features such as brand, processor, RAM, storage type (HDD/SSD), screen size, and operating system to estimate the price of a laptop. The project includes data preprocessing, feature engineering, model training, and evaluation, with a user-friendly interface for price prediction.

## Features
- **Data Preprocessing**: Cleaning and transforming laptop specifications, including one-hot encoding for categorical features and handling missing values.
- **Machine Learning Models**: Utilizes algorithms like Random Forest Regressor or Linear Regression for accurate price predictions.
- **Dataset**: Based on a dataset of approximately 1300 laptops with features like brand, CPU, RAM, storage, and price.
- **User Interface**: (Optional) A web-based interface using Streamlit for inputting laptop specifications and viewing predicted prices.

## Requirements
To run this project, you need the following dependencies:
- Python 3.8+
- Libraries:
  - `numpy`
  - `pandas`
  - `scikit-learn`
  - `streamlit` (if using the web interface)
  - `matplotlib` (for visualization)

Install dependencies using:
```bash
pip install -r requirements.txt
```

## Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/pallavisuthar03-coder/Laptop-price-predictor-.git
   cd Laptop-price-predictor-
   ```

2. **Install Dependencies**:
   ```bash
   pip install numpy pandas scikit-learn streamlit matplotlib
   ```

## Usage
1. **Prepare the Dataset**:
   - Place the dataset (e.g., `laptop_data.csv`) in the project directory.
   - Expected columns: Company, Type, RAM, Storage (HDD/SSD), CPU, GPU, OS, Screen Size, Weight, Price, etc.

2. **Run the Model**:
   - Execute the main script (e.g., `laptop_price_predictor.py`) to preprocess data, train the model, and evaluate performance:
     ```bash
     python laptop_price_predictor.py
     ```

3. **Run the Web App** (if applicable):
   - Launch the Streamlit app:
     ```bash
     streamlit run app.py
     ```
   - Open your browser and go to `http://localhost:8501` to input laptop specifications and get price predictions.

4. **Example**:
   - Input: Brand=Apple, RAM=16GB, SSD=512GB, Screen Size=13.3 inches
   - Output: Predicted price (e.g., $1200)

## Project Structure
- `laptop_price_predictor.py`: Main script for data preprocessing, model training, and evaluation.
- `app.py`: (Optional) Streamlit web app for interactive price predictions.
- `requirements.txt`: List of required Python libraries.
- `data/`: Directory for the dataset (e.g., `laptop_data.csv`).
- `models/`: Directory for saving trained models (e.g., `pipe.pkl`).

## Results
- The model achieves high accuracy (e.g., ~85-90% R² score with Random Forest, based on typical project performance).
- Evaluation metrics include Mean Absolute Error (MAE), Mean Squared Error (MSE), and R² score.



