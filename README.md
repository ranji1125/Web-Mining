# Web-Mining

## Project Overview

This repository contains the implementation and findings from the research project titled "A Comparative Analysis of Transformer and Latent Factor Models with Sentiment Analysis for Rating Prediction in Recommender Systems". Conducted by a team of researchers from the University of California, San Diego, this project explores the effectiveness of different machine learning models in predicting user ratings within recommender systems.

## Repository Structure

```
/repo_root
│
├── /data                   # Dataset and preprocessing scripts
│   ├── preprocess.py
│   └── dataset.csv
│
├── /models                 # Model implementation files
│   ├── transformer.py
│   └── latent_factor.py
│
├── /results                # Output results and figures
│   ├── performance_metrics.csv
│   └── visualizations.png
│
└── README.md               # Project documentation
```

## Models

### Transformer Model

- **Description**: Implements the Transformer model architecture to handle sequential text data from reviews.
- **Input**: Review texts.
- **Output**: Predicted ratings based on textual analysis.

### Latent Factor Model

- **Description**: Utilizes both user-business interactions and review texts, incorporating sentiment scores to enhance prediction accuracy.
- **Input**: User IDs, business IDs, and review texts.
- **Output**: Predicted ratings with enhanced understanding from sentiment analysis.

## Data

The dataset comprises Google Restaurant reviews, categorized into training, validation, and testing sets with respective sizes of 87,013, 10,860, and 11,015 reviews. This data is instrumental in training and validating the models.

## Sentiment Analysis

Utilizing VADER (Valence Aware Dictionary and sEntiment Reasoner), the project integrates sentiment scores into the Latent Factor Model, providing a nuanced interpretation of textual feedback in correlation with user ratings.

## Performance

The effectiveness of the models is measured using Mean Squared Error (MSE). Findings show that while Transformers are adept at handling complex text data, Latent Factor Models, augmented with sentiment analysis, offer a more computationally efficient and accurate approach for rating predictions.

## Installation and Running Scripts

To replicate the findings or further develop the models, follow these steps:

1. Clone the repository.
2. Ensure Python 3.6+ is installed.
3. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
4. Run preprocessing to prepare the data:
   ```
   python preprocess.py
   ```
5. Execute the model scripts:
   ```
   python transformer.py
   python latent_factor.py
   ```

## Conclusion

The project underscores the advantages of integrating sentiment analysis into Latent Factor Models for rating prediction in recommender systems, highlighting the balance between computational efficiency and predictive accuracy.
