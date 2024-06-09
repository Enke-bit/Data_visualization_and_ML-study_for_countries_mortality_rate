Health Statistics Analysis and Forecasting
Introduction
This project aims to analyze and forecast health statistics using a dataset containing various health indicators from the World Health Organization (WHO). The dataset includes information on life expectancy, maternal mortality, child mortality, infectious and non-communicable diseases, substance abuse, road traffic injuries, sexual and reproductive health, universal health coverage, environmental pollution, tobacco control, health workforce, violence against women, drinking water, sanitation, hygiene, and clean household energy.

The project uses regression-based machine learning techniques to model and predict future health statistics based on historical data.

Dataset Description
The dataset includes the following categories and their corresponding CSV files:

Life Expectancy and Healthy Life Expectancy
lifeExpectancyAtBirth.csv: Life expectancy at birth by country.
HALElifeExpectancyAtBirth.csv: Healthy life expectancy at birth by country.
WHOregionLifeExpectancAtBirth.csv: Life expectancy at birth by WHO region.
HAleWHOregionLifeExpectancy.csv: Healthy life expectancy at birth by WHO region.
%HaleInLifeExpectancy.csv: Percentage of HALE in life expectancy.

Maternal Mortality
MotherMortalityRatio.csv: Maternal mortality ratio per 100,000 live births.
AttendingBySkilledPersonal.csv: Births attended by skilled health personnel (%).

Neonatal and Child Mortality
infantMortalityRate.csv: Infant mortality rate per 1,000 live births.
neonatalMortalityRate.csv: Neonatal mortality rate per 1,000 live births.
under5MortalityRate.csv: Under-5 mortality rate per 1,000 live births.

Infectious Diseases
incedenceOfMalaria.csv: Malaria incidence per 1,000 population at risk.
incedenceOfTuberculosis.csv: Tuberculosis incidence per 100,000 population.
hepatitusBsurfaceAntigen.csv: Prevalence of Hepatitis B surface antigen in children under 5.
müdahaleAgianstNTD's.csv: Number of people requiring interventions against neglected tropical diseases (NTDs).
newHivInfections.csv: New HIV infections per 1,000 uninfected population.
Non-communicable Diseases and Mental Health
30-70cancerChdEtc.csv: Probability of dying between age 30 and exact age 70 from cardiovascular disease, cancer, diabetes, or chronic respiratory disease.
hamSuicideRates.csv: Crude suicide rates per 100,000 population.

Substance Abuse
AlcoholSubstanceAbuse.csv: Total (recorded + unrecorded) alcohol consumption per capita (15+).

Road Traffic Injuries
roadTrafficDeaths.csv: Estimated road traffic death rate per 100,000 population.

Sexual and Reproductive Health
reproduktifAgeWomen.csv: Proportion of married or in-union women of reproductive age whose family planning needs are met with modern methods (%).
adolesBirthRate.csv: Adolescent birth rate per 1,000 women aged 15-19.

Universal Health Coverage
uhcCoverage.csv: UHC service coverage index (SCI).
dataAvailibilityForUhc.csv: Data availability for UHC service coverage index (%).
nüfus10%SDG3.8.2.csv: Proportion of population with household expenditures on health greater than 10% of total household expenditure or income (%).
nüfus25%SDG3.8.2.csv: Proportion of population with household expenditures on health greater than 25% of total household expenditure or income (%).

Environmental Pollution
airPollutionDeathRate.csv: Death rate attributable to ambient and household air pollution per 100,000 population.
mortaliteRateUnsafeWash.csv: Mortality rate attributable to unsafe WASH services per 100,000 population.
mortaliteRatePoisoning.csv: Mortality rate attributable to unintentional poisoning per 100,000 population.

Tobacco Control
tütünAge15.csv: Prevalence of tobacco use among persons aged 15 and older.

Health Workforce
MedicalDoctors.csv: Medical doctors per 10,000 population.
nurseAndMidwife.csv: Nursing and midwifery personnel per 10,000 population.
Dentists.csv: Dentists per 10,000 population.
Pharmacists.csv: Pharmacists per 10,000 population.

Violence Against Women
elimineViolenceAgainstWomen.csv: Proportion of ever-partnered women and girls aged 15-49 subjected to physical and/or sexual violence by a current or former intimate partner in the previous 12 months (%).

Drinking Water
basicDrinkingWaterServices.csv: Population using at least basic drinking water services (%).

Sanitation and Hygiene
atLeastBasicSanitizationServices.csv: Population using at least basic sanitation services (%).
secureSanitization.csv: Population using safely managed sanitation services (%).
basicHandWashing.csv: Population with basic handwashing facilities on premises (%).

Clean Household Energy
cleanFuelAndTech.csv: Population primarily relying on clean fuels and technologies (%).

Installation
To run the analysis and forecasting, you need to install the following Python packages:

pandas
seaborn
matplotlib
scikit-learn
Data Preprocessing
The preprocessing steps involve handling missing values, removing non-numeric columns, converting categorical variables to numeric using one-hot encoding, and ensuring the target variable is numeric.

Model Building
A regression model is built using the LinearRegression class from the scikit-learn library. The model is trained on the historical data to learn the relationships between features and the target variable.

Evaluation
The model's performance is evaluated using Mean Squared Error (MSE) and R-squared (R²) metrics to measure the accuracy and goodness of fit.

Future Predictions
Once the model is trained and evaluated, it can be used to make future predictions based on new input data. Ensure the new data has the same structure as the training data, including any necessary preprocessing steps.

Usage
Load the dataset.
Inspect and clean the data.
Split the data into training and testing sets.
Build and train the model.
Evaluate the model's performance.
Make future predictions based on new data.
