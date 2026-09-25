# sales-weather-analysis
Group project: how daily temperature relates to restaurant sales (pandas, matplotlib for MBA 561 Introduction to Applied Business Analytics course


This team project looks at whether weather drives sales at a multi-location restaurant chain. We worked with two datasets: 438,151 point-of-sale line items from 2014 to 2017 (items, departments, stores, prices, quantities and totals) and a year of daily maximum temperatures for 2016, stored in wide weekly format.

Using pandas, we converted date fields to datetime and removed 12 records with missing price values (under 0.003% of the data). We summed the transactions into daily totals of quantity and revenue. We reshaped the weather data from wide to long format and built a calendar date for each reading from the week-start date plus a weekday offset. An inner join on date then produced 311 days in 2016 with both sales and temperature data.

Scatter plots showed no clear relationship between temperature and either revenue or units sold. The highest-sales days fell across cool and warm temperatures alike, which suggests factors like day of week, promotions or seasonality matter more. As expected, quantity and revenue showed a strong positive relationship.

Tools: Python, pandas, matplotlib, Jupyter, PyArrow
