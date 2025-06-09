# DL2025-SentimentAnalysis

Final project for the 2025 Deep Learning course at Universitat Pompeu Fabra.

## Project Overview

This project aims to build a sentiment analysis LSTM-based model to classify text for detecting potential mental health issues. The workflow is divided into three main parts:
1. **Exploratory Data Analysis (EDA)**
2. **Preprocessing optimization**
3. **Model architecture optimization**

All the preprocessing and model architecture optimization is performed iteratively: for each change in preprocessing or model design, we test its effect on the model. If the change improves results, it is added to the best model and further improvements are tested on top; if not, the change is discarded.

## Environment Setup

1. **Python Version**: 3.8 or higher is recommended.
2. **Recommended Platform**: Google Colab (for easy access to GPU and Google Drive integration), but it can also run locally.

## Dependencies

Install the following Python packages:

- pandas
- numpy
- matplotlib
- seaborn
- torch
- tensorflow / keras
- nltk
- scikit-learn
- wordcloud

If you are not working on Google Colab, consider using the installation guide on (https://pytorch.org/) to properly install PyTorch with GPU integration 

You can install the rest using pip:

```sh
pip install pandas numpy matplotlib seaborn torch tensorflow nltk scikit-learn wordcloud
```

## Data

- Download the dataset `sentiment_analysis_data.csv` and place it in the `data/` directory.
- If using GloVe embeddings, download the required GloVe files (e.g., `glove.6B.100d.txt` and `glove.6B.200d.txt`) from [https://nlp.stanford.edu/projects/glove/](https://nlp.stanford.edu/projects/glove/) and place them also in the `data/` directory.

## Running the Notebooks

1. **Exploratory Data Analysis**:
   Open and run all cells in `EDA_FinalProject_TeamH.ipynb` to explore and preprocess the data.

2. **Experiments**:
   Open and run all cells in `Models_FinalProject_TeamH.ipynb` to train the LSTM-based models and evaluate their performance.

3. **Results**:
   Output figures and model artifacts will be saved in the `results/` directory.

## Notes

- If running on Google Colab, make sure to mount your Google Drive to access data and save results.
- **Adjust file paths** as needed if running locally.
