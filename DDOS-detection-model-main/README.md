

# DDoS Attack Detection using Random Forest

This repository contains an AI model built to detect Distributed Denial-of-Service (DDoS) attacks in network traffic using the Random Forest algorithm. The model preprocesses network traffic data and identifies whether it is benign or malicious based on labeled data.

## Project Overview

This project uses machine learning techniques, specifically **Random Forest**, to identify patterns associated with DDoS attacks. The model processes network traffic data and classifies it as benign or malicious, enabling early detection and mitigation of DDoS attacks.

## Dataset

The dataset used for training and testing the model is a CSV file (`ddos1.csv`) that includes features related to network traffic, such as:
- Packet rate
- Inter-arrival time
- Packet size
- Duration
- Source and destination ports
- Number of packets and bytes transferred
- Protocol type (converted into dummy variables)
  
The dataset contains a **label** column that indicates whether the traffic is benign or part of a DDoS attack.

## Requirements

The project requires the following Python libraries:
- pandas
- scikit-learn
- seaborn
- matplotlib

To install the required dependencies, run:

```bash
pip install -r requirements.txt
```

## File Structure

- `ddos1.csv`: The dataset used for training and testing.
- `ddos1.ipynb`: The Jupyter notebook containing the DDoS detection implementation.
- `requirements.txt`: A file listing all the necessary Python libraries.

## How to Use

1. Clone the repository to your local machine.
2. Install the necessary dependencies by running:
   ```bash
   pip install -r requirements.txt
   ```
3. Place your `ddos1.csv` dataset in the same directory as the notebook.
4. Open and run the `ddos1.ipynb` Jupyter notebook.
5. The notebook will preprocess the data, train the Random Forest model, and output the following:
   - Accuracy score of the model
   - Classification report (precision, recall, F1-score)
   - Confusion matrix visualization
   - Feature importance plot

## Model Performance

After training, the model evaluates its performance on the test set. The key evaluation metrics include:
- **Accuracy**: Proportion of correct predictions (benign or malicious).
- **Precision, Recall, F1-Score**: Detailed classification metrics for both benign and malicious traffic.
- **Confusion Matrix**: A visual representation of true positive, true negative, false positive, and false negative predictions.
- **Feature Importance**: A plot showing which features contribute most to the model's decisions.

## Example Output

- **Accuracy**: 95.67%
- **Classification Report**: Detailed breakdown of precision, recall, and F1 scores for both classes (benign and malicious).
- **Confusion Matrix**: A heatmap showing the actual vs. predicted values.
- **Feature Importance**: A bar chart visualizing the importance of different features used for model decision-making.

## Contribution

Feel free to contribute to this project by:
- Reporting issues
- Submitting pull requests for improvements or bug fixes

