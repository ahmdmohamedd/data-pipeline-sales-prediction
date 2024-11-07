# Data Pipeline for Sales Prediction

This repository contains a comprehensive data pipeline for sales prediction using Dask and Pandas. The pipeline processes large datasets, performs feature engineering, applies preprocessing techniques, and trains a model using HistGradientBoostingRegressor. It is designed to handle high volumes of data, optimize performance, and deliver predictions for sales forecasting.

## Key Features
- **Data Loading**: Efficient data handling using Dask for large datasets.
- **Data Preprocessing**: Handling missing values, converting datatypes, and creating new features.
- **Feature Engineering**: Creation of additional features such as `trip_duration` and removal of outliers.
- **Model Training**: Utilizes HistGradientBoostingRegressor for regression tasks.
- **Evaluation**: Model performance is evaluated using metrics such as R², MSE, and MAE.
- **Visualization**: Interactive visualizations to inspect feature distributions and model performance.

## Dataset Information
The dataset used in this project contains the following columns:
- `VendorID`
- `tpep_pickup_datetime`
- `tpep_dropoff_datetime`
- `passenger_count`
- `trip_distance`
- `pickup_longitude`
- `pickup_latitude`
- `RatecodeID`
- `store_and_fwd_flag`
- `dropoff_longitude`
- `dropoff_latitude`
- `payment_type`
- `fare_amount`
- `extra`
- `mta_tax`
- `tip_amount`
- `tolls_amount`
- `improvement_surcharge`
- `total_amount`

### Note on Dataset Files
Due to the size of the processed data, the `pca_components.csv` and `processed_yellow_taxi_data.csv` files are too large to upload to this repository. However, these files are generated during the pipeline execution and can be saved locally after running the notebook.

## Installation

To use this system, ensure you have the following installed:
- Python 3.x
- Jupyter Notebook or JupyterLab
- Dask
- Pandas
- scikit-learn
- Matplotlib
- Seaborn

You can install the required libraries using `pip` or `conda`:

```bash
# Using pip
pip install pandas dask scikit-learn matplotlib seaborn

# Or using conda
conda install pandas dask scikit-learn matplotlib seaborn
```

## Running the System

1. Clone this repository to your local machine:
    ```bash
    git clone https://github.com/ahmdmohamedd/data-pipeline-sales-prediction.git
    ```

2. Navigate to the project directory:
    ```bash
    cd data-pipeline-sales-prediction
    ```

3. Open the Jupyter notebook:
    ```bash
    jupyter notebook data-pipeline-sales-prediction.ipynb
    ```

4. Follow the instructions in the notebook to run the pipeline. The notebook will walk you through data loading, preprocessing, feature engineering, model training, and evaluation.

## Expected Outputs

- The pipeline will generate the following files:
  - `pca_components.csv`: Contains the principal components after applying PCA for dimensionality reduction.
  - `processed_yellow_taxi_data.csv`: Processed data with cleaned and engineered features.
  
  These files will be saved in the same directory where the notebook is executed.

## Contributing

Feel free to fork this repository, open issues, and submit pull requests. Any contributions or improvements to the code are welcome!
