# Know-Your-Air-PM2.5-Prediction-with-LIME
"Transparent AI models for interpretable forecasting of PM2.5 air pollution using explainable machine learning techniques."
This project leverages interpretable machine learning techniques to forecast PM2.5 air pollution levels and provides clear, actionable insights via model explainability. Using LIME, we highlight how input features influence predictions, creating transparency for researchers, developers, and decision makers.
## Features

- Robust data import supporting both image and tabular air quality datasets  
- Comprehensive data exploration including statistical summaries and visualization  
- Advanced data cleaning and preprocessing techniques, including missing value handling and normalization  
- Feature engineering to extract meaningful variables and enhance model input  
- Support for multiple machine learning models such as Random Forest and XGBoost for PM2.5 prediction  
- Thorough model evaluation using key metrics (RMSE, MAE, \(R^2\)) to ensure accuracy  
- Leveraging LIME for local explanation of model predictions, enhancing interpretability  
- Detailed visualization of model outputs and explanation results for easy understanding  
- Scalable pipeline suitable for environmental monitoring and air quality forecasting applications
## Model Flow
The following diagram illustrates the complete workflow of the Know-Your-Air-PM2.5-Prediction-with-LIME model:

Know-Your-Air-PM2.5-Prediction-with-LIME Model Workflow
![Banner](https://github.com/anusha-buchipalli/Know-Your-Air-PM2.5-Prediction-with-LIME/blob/main/generated-image.png?raw=true)
The workflow consists of eight main stages:
1. **Data Preparation**  
   - Import raw air quality datasets (image/tabular).  
   - Perform data cleaning and preprocessing including missing value imputation and normalization.  

2. **Feature Engineering**  
   - Generate relevant features such as lag variables, statistical summaries, or image-derived metrics.  
   - Encode categorical variables if any.

3. **Model Selection**  
   - Compare multiple machine learning models: Random Forest, XGBoost, LightGBM, etc.  
   - Fine-tune hyperparameters for optimum performance.

4. **Model Training**  
   - Train models on prepared datasets.  
   - Apply cross-validation or train-test splits for validation.

5. **Prediction**  
   - Generate PM2.5 concentration predictions on test or new data.

6. **Explainability with LIME**  
   - Apply LIME algorithm to interpret and explain individual predictions.  
   - Examine feature contributions to prediction outcomes.

7. **Model Evaluation**  
   - Assess model accuracy using metrics such as RMSE, MAE, and \(R^2\).

8. **Result Visualization**  
   - Plot prediction results and LIME explanations to support interpretability and decision making.
## Dataset Reference

This project uses the Air Pollution Image Dataset from India and Nepal, which is publicly available on Kaggle:  
[Air Pollution Image Dataset from India and Nepal](https://www.kaggle.com/datasets/adarshrouniyar/air-pollution-image-dataset-from-india-and-nepal)

This project uses the Air Pollution Image Dataset from India and Nepal, containing 12,240 images with a size of 224x224 pixels.

The dataset is organized into two main folders:

- **Combined_Dataset:**  
  - `All_img`: Contains all collected images across AQI classes.  
  - `IND_and_NEP`: Contains six subfolders representing different AQI classes.  
  - Includes a CSV file labeling each image with parameters such as Location, Filename, Year, Month, Day, Hour, AQI, PM2.5, PM10, O3, CO, SO2, NO2, and AQI_Class.

- **Country_wise_Dataset:**  
  - Divided into two subfolders: India and Nepal.  
  - Each country's folder contains city-wise subfolders.  
  - Each city folder has further subfolders for each AQI class and an associated CSV file with detailed image metadata (same parameters as above).

### Cities in the Dataset

- India: ITO (Delhi), Dimapur (Nagaland), Spice Garden (Bengaluru), Knowledge Park III (Greater Noida), New Industrial Town (Faridabad), Borivali East (Mumbai), Oragadam (Tamil Nadu)  
- Nepal: Biratnagar

This structured dataset forms the basis for training and testing machine learning models in this project.

