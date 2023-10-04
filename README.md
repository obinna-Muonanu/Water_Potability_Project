# Water_Potability_Project
![image](https://github.com/obinna-Muonanu/Water_Potability_Project/assets/96579075/1d12aa8d-221f-4cbf-b6b4-6e5254f81375)
## Description
Ensuring access to safe drinking water is a fundamental human right and a key component of effective health protection policies. It holds immense importance at local, regional, and national levels, impacting both health and development.
Moreover, in certain regions, investing in clean water supply and sanitation has demonstrated a positive economic impact. The reduction in health-related issues and healthcare costs resulting from these investments outweighs the initial expenses, ultimately leading to a net economic benefit.
This report provides a concise overview of this predictive model designed to determine water potability. 
## Introduction
This report presents the findings and analysis of five machine learning models namely:

-	Random Forest
-	Logistic Regression
-	XGBoost
-	Lightgbm
-	Catboost


To predict if water is potable for drinking or not. 
A water potability predictive model is incredibly valuable to society because it helps keep our drinking water safe. It identifies whether the water we're about to drink is safe or not, allowing us to take action to avoid getting sick from contaminated water. By catching potential problems early, it helps prevent water-related illnesses, reducing healthcare costs and saving individuals from medical bills. This predictive model help keep us healthy, save money, and ensure that we can rely on our water supply, benefiting everyone in society. The primary aim of this model is to effectively predict if the water sample is portable or not based on the following features:

-	pH value
-	Hardness
-	Solids (Total dissolved solids - TDS)
-	Chloramines
-	Sulfate
-	Conductivity
-	Organic_carbon
-	Trihalomethanes
-	Turbidity

## Dependencies
The following python packages are required to run the code:
- Numpy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn
- RandomForestClassifier
- LogisticRegression
- XGBoost
- Lightgbm
- CatBoost

## Exploratory Data Analysis
I conducted exploratory data analysis to gain a good understanding of the dataset and gain insights  from it. This knowledge was used in building and training the machine learning model.
### Data Source and Description
The dataset was gotten from Kaggle Datasets.
The dataset contains information about the water quality parameters that will enable the model predict if the water is potable or not. The dataset contains 3276 entries and 10 columns.
The features in the dataset include:
#### pH value:
PH is an important parameter in evaluating the acid–base balance of water. It is also the indicator of acidic or alkaline condition of water status. WHO has recommended maximum permissible limit of pH from 6.5 to 8.5. The current investigation ranges were 6.52–6.83 which are in the range of WHO standards.
##### Hardness:
Hardness is mainly caused by calcium and magnesium salts. These salts are dissolved from geologic deposits through which water travels. The length of time water is in contact with hardness producing material helps determine how much hardness there is in raw water. Hardness was originally defined as the capacity of water to precipitate soap caused by Calcium and Magnesium.
##### Solids (Total dissolved solids - TDS):
Water has the ability to dissolve a wide range of inorganic and some organic minerals or salts such as potassium, calcium, sodium, bicarbonates, chlorides, magnesium, sulfates etc. These minerals produced un-wanted taste and diluted color in appearance of water. This is the important parameter for the use of water. The water with high TDS value indicates that water is highly mineralized. Desirable limit for TDS is 500 mg/l and maximum limit is 1000 mg/l which prescribed for drinking purpose.
##### Chloramines:
Chlorine and chloramine are the major disinfectants used in public water systems. Chloramines are most commonly formed when ammonia is added to chlorine to treat drinking water. Chlorine levels up to 4 milligrams per liter (mg/L or 4 parts per million (ppm)) are considered safe in drinking water.
##### Sulfate:
Sulfates are naturally occurring substances that are found in minerals, soil, and rocks. They are present in ambient air, groundwater, plants, and food. The drinking standards laid down by the WHO are 250 mg/L of sulfates and the maximum admissible concentration can reach 400 mg/L.
##### Conductivity:
Pure water is not a good conductor of electric current rather it is a good insulator. Increase in ions concentration enhances the electrical conductivity of water. Generally, the amount of dissolved solids in water determines the electrical conductivity. Electrical conductivity (EC) actually measures the ionic process of a solution that enables it to transmit current. According to WHO standards, EC value should not exceeded 400 μS/cm.
##### Organic carbon:
Total Organic Carbon (TOC) in source waters comes from decaying natural organic matter (NOM) as well as synthetic sources. TOC is a measure of the total amount of carbon in organic compounds in pure water. According to US EPA < 2 mg/L as TOC in treated / drinking water, and < 4 mg/Lit in source water which is use for treatment.
##### Trihalomethanes:
THMs are chemicals which may be found in water treated with chlorine. The concentration of THMs in drinking water varies according to the level of organic material in the water, the amount of chlorine required to treat the water, and the temperature of the water that is being treated. THM levels up to 80 ppm is considered safe in drinking water.
##### Turbidity:
The turbidity of water depends on the quantity of solid matter present in the suspended state. It is a measure of light emitting properties of water and the test is used to indicate the quality of waste discharge with respect to colloidal matter. The mean turbidity value obtained for Wondo Genet Campus (0.98 NTU) is lower than the WHO recommended value of 5.00 NTU.

##### Below is a summary statistics of the features in the dataset
![image1](https://github.com/obinna-Muonanu/Water_Potability_Project/assets/96579075/820d5ce5-dbd9-4b53-8487-2d4948bb832a)
![Image2](https://github.com/obinna-Muonanu/Water_Potability_Project/assets/96579075/860e61ff-f496-4b07-b1f2-067e3dad9ca5)
![image5](https://github.com/obinna-Muonanu/Water_Potability_Project/assets/96579075/c0d61856-abbc-4bcf-bc72-5ead5087687d)

## Data Preprocessing
Prior to building the predictive model, the dataset underwent different preprocessing steps including:
- Handling missing values
- Handling class imbalance in the target variable
- Handling Outliers
- Feature Engineering
- Encoding Categorical Variables
- Feature Scaling

## Model
Five different machine learning models were trained on the train dataset. The project includes a jupyter notebook that demonstrates the data preprocessing, model training, and evaluation steps.

## Evaluation
The model's performance is evaluated using the accuracy_score and precision_score
### Below are the results from the validation dataset

- ###### Model -- Random Forest
- ###### Accuracy score --  0.7575135218667903
- ###### Precision score -- 0.7808988764044944
- ###### Model -- Logistic Regression
- ###### Accuracy score --  0.5108379694019471   
- ###### Precision score -- 0.465625
- ###### Model -- XGBoost
- ###### Accuracy score --  0.7411060887034462
- ###### Precision score -- 0.725130890052356
- ###### Model -- CatBoost
- ###### Accuracy score --  0.7406886493586773 
- ###### Precision score -- 0.7506631299734748 
- ###### Model -- LightGBM
- ###### Accuracy score --  0.7419371040024727 
- ###### Precision score -- 0.7405405405405405

### Below are the accuracy scores on the test datasets
- ###### Model -- Random Forest
- ###### Accuracy score --  0.725

- ###### Model -- Logistic Regression
- ###### Accuracy score --  0.4625  

- ###### Model -- XGBoost
- ###### Accuracy score --  0.72

- ###### Model -- CatBoost
- ###### Accuracy score --  0.7

- ###### Model -- LightGBM
- ###### Accuracy score --  0.72 


## Acknowledgements
The daataset used for this project was sourced from Kaggle Datasets.
