# apnea_detection

## Overview
This project aims to develop a machine learning model to detect apnea using physiological signals. Apnea, a potentially serious sleep disorder, involves periods during which breathing stops or becomes shallow during sleep. Early detection is crucial for effective management and treatment.

## Data Source
Data for this project is sourced from the Sleep Heart Health Study database available at [PhysioNet](https://physionet.org/content/slpdb/1.0.0/). This dataset includes physiological signals recorded during sleep such as ECG, BP, and EEG, which are instrumental in diagnosing sleep disorders like apnea.

## Methodology
### Data Preprocessing
Data from each patient is processed to extract relevant signals (ECG, BP, EEG) and segment these into 30-second windows, aligning with the standard measurement periods used in sleep studies. This preprocessing is crucial for the consistency and accuracy of feature extraction.

### Model Architecture
The core of our analysis is built on a deep learning model using LSTM (Long Short-Term Memory) layers. This model architecture is designed to capture temporal dependencies in the physiological signals, which are pivotal for detecting patterns indicative of apnea.

### Latent Space Representation
To understand the model's behavior and ensure it correctly identifies features relevant to apnea detection, we project the high-dimensional data onto a 2D space using t-SNE (t-Distributed Stochastic Neighbor Embedding). This visualization helps in assessing the model's ability to segregate the data based on the presence or absence of apnea.

### Performance Evaluation
The model's performance is evaluated using a confusion matrix, and results are visualized to verify sensitivity and specificity in distinguishing between apneic and non-apneic episodes. The classification report provides a detailed account of accuracy, recall, precision, and F1-score.

## Usage
The repository includes a Jupyter Notebook that outlines the entire process from data loading and preprocessing, through model training and evaluation, to final visualizations of the model's performance. Users can follow these steps to replicate the study or use the methodology as a basis for further research.

## Contributing
Contributions to this project are welcome. You can contribute by improving the existing model, extending the dataset, or suggesting new features. Please ensure to follow the existing coding style and add comments to your modifications.

## License
This project is open source and available under the MIT License.