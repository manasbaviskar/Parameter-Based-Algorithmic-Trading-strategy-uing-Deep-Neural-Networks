# Deep Learning-based Algorithmic Trading Strategy

This project involves a deep learning-based algorithmic trading strategy using historical stock price data. The model leverages statistical, trend-related, and momentum-based features to predict the movement of stock prices. The core of the model is a Multi-layer Perceptron Classifier (MLP), and the strategy was tested on **Microsoft** stock data.

## Methodology

### Feature Engineering
To predict stock price movements, a variety of technical indicators and statistical features were created:
- **Statistical Features**: Standard deviation, moving averages of different window sizes, percentage changes in closing prices.
- **Technical Indicators**: Bollinger Bands, Moving Average Convergence Divergence (MACD), Parabolic Stop And Reverse (SAR).

These features were used to train a **Multi-layer Perceptron (MLP) Classifier**.

### Model Architecture
- **Model Type**: Multi-layer Perceptron Classifier (MLP)
- **Hidden Layer**: 1 hidden layer with 5 neurons
- **Library Used**: Scikit-learn for MLP Classifier

### Training & Back-testing
- **Training**: The model was trained on historical stock data for Microsoft.
- **Testing**: Accuracy was evaluated on both training and testing datasets, ensuring the model generalizes well and does not overfit.
- **Back-testing**: Simulated real-world trading by applying the model to historical stock data and comparing its performance with a simple buy-and-hold strategy.

## Installation Instructions
Clone the repository and install the required dependencies:

```bash
git clone https://github.com/yourusername/deep-learning-algorithmic-trading.git
cd deep-learning-algorithmic-trading
pip install -r requirements.txt
```

## Usage
To train the model, simply run:

```bash
python train_model.py
```

For back-testing the strategy, run:

```bash
python backtest_strategy.py
```

Ensure that the necessary stock data is available in the `data/` folder or fetch it using the script provided in the repository.

## Results
The model outperformed a simple buy-and-hold strategy by **9.4%** during back-testing. The back-testing results can be found in the `results/` folder, including performance metrics and visualizations.

## Technologies Used
- **Python** (Numpy, Pandas, Scikit-learn)
- **MLP Classifier** from scikit-learn
- **Matplotlib** and **Seaborn** for data visualization
- **Jupyter Notebooks** for exploration and prototyping
- **pandas_datareader** for fetching historical stock data

---

Feel free to modify the project title, structure, and details according to your specific setup!
