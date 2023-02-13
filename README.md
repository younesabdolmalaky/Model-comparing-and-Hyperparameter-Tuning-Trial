# Model-comparing-and-Hyperparameter-Tuning-Trial
# About the dataset
The data points were collected from a Combined Cycle Power Plant over 6 years (2006-2011) when the power plant was set to work with a full load. Features consist of hourly average ambient variables - Ambient Temperature (AT), Ambient Pressure (AP), Relative Humidity (RH) and Exhaust Vacuum (V) to predict the net hourly electrical energy output (PE) of the plant.

A combined-cycle power plant uses both gas and a steam turbine together to produce up to 50 percent more electricity from the same fuel than a traditional simple-cycle plant. The waste heat from the gas turbine is routed to the nearby steam turbine, which generates extra power.

All the UN Member States have to submit a report on the combined cycle power plant to the United Nations. The Power Plant officials of Mexico are devising a way to predict the net hourly electrical energy output (PE) of the plant. You are appointed as the chief for this operation. Create a Machine Learning Model to solve this problem efficiently.

#Introduction¶

Single-cycle gas turbine power plants generate electricity by using natural gas and compressed air. Air is drawn from the surroundings, compress ed, and fed into the combustion chamber of the gas turbine. Here, natural gas is injected which mixes with the compressed air and ignited. The combustion produces a high-pressure, hot gas stream that flows through the turbine causing it to spin (at tremendous speeds). Consequently, this spins a generator which is connected to the turbine to produce electricity. For single-cycle gas turbines, much of the energy is wasted as hot exhaust achieving an energy conversion efficiency of 35% at best. Combined cycle power plants exploit this inefficiency by capturing the waste heat using a heat recovery steam generator (HRSG), to produce even more power. Combined cycle power plants are power generation plants that use both gas and steam turbines together to generate electricity. The waste heat generated from the gas turbine is used to produce steam which is fed to a steam turbine to generate even more electricity. This increases the power produced (up to 50% more) for the same amount of fuel, as well as increases the plant’s efficiency to about 60%. The Output power of the Combined Cycle Power Plant (CCPP) is dependent on a few parameters which are atmospheric pressure, exhaust steam pressure, ambient temperature, and relative humidity. Being able to predict the full load electrical power output is important for the efficient and economic operation of the power plant.

![download](https://user-images.githubusercontent.com/75095471/217403841-9d5596d8-0224-4a76-bbe3-97788a9600cd.png)

# Algorithms Overview
Model Evaluation for Regression Task
In this evaluation, eight different algorithms were used for a regression problem:
<ul class="myUL">
  <li>Decision Tree Regressor</li>
  <li>Random Forest Regressor</li>
  <li>K-Nearest Neighbors Regressor</li>
   <li>Support Vector Regression (SVR)</li>
  <li>CatBoost Regressor</li>
  <li>XGBoost Regressor</li>
  <li>Deep Learning Neural Network (MLP)</li>
</ul>

Each model was fit to the training data and then used to make predictions on the test data. The evaluation metrics used were the R2-score and the Mean Absolute Error (MAE). The R2-score is a measure of how well the model fits the data, with a score of 1.0 indicating a perfect fit and a score of 0.0 indicating a poor fit. The MAE is a measure of the average error between the actual values and the predicted values.
The results of the model evaluation are presented in the table below:

<table>
  <tr>
    <th>Model name</th>
    <th>R2-score</th>
    <th>MAE</th>
    <th>Time (seconds)</th>
  </tr>
  <tr>
    <td>Linear Regression</td>
    <td>0.924769</td>
    <td>3.669618</td>
    <td>0.029593</td>
  </tr>
  <tr>
    <td>Decision Tree</td>
    <td>0.921349</td>
    <td>3.313986</td>
    <td>0.045285</td>
  </tr>
  <tr>
    <td>Random Forest</td>
    <td>0.955716</td>
    <td>2.526763</td>
    <td>2.827737</td>
  </tr>
  <tr>
    <td>K-Nearest Neighbors</td>
    <td>0.941989</td>
    <td>3.001490</td>
    <td>0.015856</td>
  </tr>
  <tr>
    <td>SVR</td>
    <td>0.936554</td>
    <td>3.240146</td>
    <td>1.661543</td>
  </tr>
  <tr>
    <td>CatBoost</td>
    <td>0.950686</td>
    <td>2.768416</td>
    <td>15.061745</td>
  </tr>
  <tr>
    <td>XGBoost</td>
    <td>0.943266</td>
    <td>3.055684</td>
    <td>0.577507</td>
  </tr>
  <tr>
    <td>Deep Learning Neural Network</td>
    <td>0.928563</td>
    <td>3.521634</td>
    <td>34.228411</td>
  </tr>
</table>

![download (5)](https://user-images.githubusercontent.com/75095471/218534817-5eac4552-5435-4dfb-9c71-6fb33bc4ad38.png)



