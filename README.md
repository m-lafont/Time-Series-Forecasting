# Time Series Forecasting 

## Overview
This project was part of the Artificial Neural Networks and Deep Learning (AN2DL) course for 2023-2024. The objective was to develop a forecasting model capable of predicting future samples of time series data across six categories.

The final model uses a dual-branch neural network with LSTM and self-attention mechanisms. Advanced preprocessing techniques, including windowing and data balancing, were applied to ensure robust performance.

---

## Features
- **Forecasting**: Predicts future samples for time series data.
- **LSTM-Based Architecture**: Dual-branch model combining LSTM and self-attention.
- **Optimization Techniques**: Includes Early Stopping, learning rate decay, and Adam optimizer.
- **Performance Tracking**: Evaluated using Mean Squared Error (MSE).

---

## Project Structure
- **`reports/Time_Series_Forecasting_Report.pdf`**: Detailed report with methodology, results, and conclusions.
- **`notebooks/Time_Series_Forecasting.ipynb`**: Jupyter Notebook for preprocessing, training, and evaluation.
  
---

## Dataset
- **Size**: 48,000 mono-variate time series of varying lengths.
- **Categories**: Six distinct categories with varying data distributions.
- **Preprocessing**:
  1. Windowing with a size of 100 time steps.
  2. Handling imbalanced categories.
  3. Removal of short time series and outliers.

---

## Methodology
1. **Model Architecture**:
   - Dual-branch design: LSTM for temporal patterns and self-attention for contextual relationships.
   - Output: Predicts up to 18 future samples.

2. **Optimization**:
   - Adam optimizer with learning rate decay.
   - Early stopping and ReduceLROnPlateau for efficient training.
   - Batch size: 128, max epochs: 200.

3. **Performance Metrics**:
   - MSE for validation and test phases.

---

## Results
- **Phase 1 (Validation)**: Achieved MSE of 0.0054.
- **Phase 2 (Test)**: Achieved MSE of 0.0102.
- Robust handling of diverse time series with minimal error.

---

## Future Improvements
- Enhance handling of short time series with masking or padding techniques.
- Improve preprocessing for outliers and missing values.
- Explore transformer-based architectures for better generalization.

---

## References
1. Eugenio Lomurno - AN2DL Labs and Logbook
2. Matteo Matteucci - Sequence-to-Sequence Learning and Transformers
