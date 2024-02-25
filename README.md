#### Predictive modeling of historical fine dust data in South Korea
Fine dust and other sources of air pollution impose a significant toll on human health, often perceived as the inevitable cost of economic prosperity. This project will utilize historical data of fine dust (PM10) concentrations, as recorded by the Suwon weather station (station number 119), to explore the following questions:

Are there significant trends such as yearly and seasonal in measured fine dust concentration?
Are there significant “one-off” events across time where fine dust levels were noticeably higher or lower than the historical record would suggest?
How do other environmental conditions, such as rainfall or traffic volume, impact fine dust concentration?
Can the observed trends and patterns in the data be extrapolated to the future?
The questions are investigated using Prophet library, https://facebook.github.io/prophet/ , as it provides modeling for time series data and allows to incorporate extra-regressors.

The historical fine dust concentration data will be divided into a train set and a test set. The Prophet model will first be applied to the train dataset and subsequently tested for its effectiveness on the test dataset. Initially, the first model will be based solely on the fine dust data. Later, a second model will incorporate additional environmental variables as extra regressors, such as rainfall or traffic volume.

The investigation begins with an examination of the historical fine dust data. The fine dust data is available in
https://data.kma.go.kr/data/climate/selectDustRltmList.do?pgmNo=68

This notebook entierly follows the methods shown in the work https://nbviewer.org/github/nicolasfauchereau/Auckland_Cycling/blob/master/notebooks/Auckland_cycling_and_weather.ipynb
