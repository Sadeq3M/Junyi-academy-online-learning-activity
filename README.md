# Junyi-Academy-Online-Learning-Analysis

## Project Overview  
This repository analyzes user engagement patterns on the **Junyi Academy** online learning platform using a comprehensive dataset of student activities, exercises, and metadata. The project explores temporal trends, problem-solving behaviors, and predictive modeling to understand factors influencing learning outcomes and platform usage.

---

## Key Insights  
1. **User Demographics**  
   - Majority of students did not specify their gender.  
   - Top cities: Taipei, New Taipei, Taichung, Kaohsiung, Taoyuan.  

2. **Behavioral Patterns**  
   - Peak usage at **4 PM**, highest activity on **Tuesdays & Thursdays**.  
   - Retention spikes after holidays (e.g., summer/winter breaks).  
   - 40% of students disengaged within **10 days**.  

3. **Exercise Analysis**  
   - Correct rates decrease with problem difficulty:  
     - **Easy**: ~80%  
     - **Hard**: ~50%  
   - Most students attempt **5-6 problems per exercise** (aligned with level-up mechanics).  

4. **Time Series Forecasting**  
   - **SARIMA** outperformed LSTM in predicting daily logins:  
     - **SARIMA RMSE**: 0.224  
     - **LSTM RMSE**: 0.335  

---

## Repository Structure  
- `/data`: Contains raw datasets (`Log_Problem.csv`, `Info_UserData.csv`, `Info_Content.csv`).  
- `/notebooks`:  
  - `EDA.ipynb`: Exploratory analysis of user behavior and exercise trends.  
  - `TimeSeries_Forecasting.ipynb`: SARIMA and LSTM models for login prediction.  
- `/results`: Visualizations (heatmaps, ACF/PACF plots, forecast comparisons).  
- `/docs`: Project report and academic calendar references.  

---

## Tools & Methods  
- **Python Libraries**: Pandas, Matplotlib, Seaborn, Statsmodels, TensorFlow/Keras.  
- **Time Series Models**:  
  - **SARIMA**: Captured seasonality and trends (optimal: `ARIMA(0,0,0)`).  
  - **LSTM**: Two-layer architecture (128/64 units).  
- **Statistical Tests**: Augmented Dickey-Fuller (ADF) for stationarity.  


--- 

## Conclusion  
The analysis highlights the impact of **academic calendars** and **exercise difficulty** on engagement. SARIMA’s superior performance suggests strong seasonal patterns in login data. Recommendations include **gamification tweaks** (e.g., adjusting energy points for harder exercises) and **targeted re-engagement campaigns** during low-activity periods.  

---  
**Note**: Dataset sourced from Junyi Academy (2018–2019). Images and plots are generated in the notebooks.
