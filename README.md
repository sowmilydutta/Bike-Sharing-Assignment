# UpGrad: BoomBikes - Bike Sharing Assignment
> **Objective:**  
> Develop a multiple linear regression model to predict demand for shared bikes. This model will help BoomBikes, a U.S.-based bike-sharing provider, analyze demand factors and adapt its business strategy to increase profitability in the post-COVID market.

> **Context:**  
> BoomBikes has experienced revenue declines due to the COVID-19 pandemic. To prepare for increased demand as restrictions lift, the company has collected data on daily bike usage influenced by various factors.  Understanding which variables most impact demand, will enable BoomBikes to stand out among competitors by meeting customer needs.

> **Goal:**  
> Analyze significant factors affecting bike demand and determine how well these variables predict demand. This insight will allow BoomBikes to fine-tune its strategies to better serve emerging demand trends and efficiently enter new markets.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information

> ### Project Overview:
> This project involves building a multiple linear regression model to predict the demand for shared bikes in the U.S. market. The primary objective is to identify key factors influencing bike demand and to understand how these factors interact with each other to affect the overall demand. The final model will allow the business to tailor its strategies based on demand predictions, potentially helping BoomBikes improve revenue and prepare for a post-pandemic recovery in demand.
>
> ### Project Background:
> Bike-sharing systems are an efficient way to provide short-term bike rentals, generally by accessing bikes from computer-controlled docks scattered around cities. With the pandemic having decreased ridership, BoomBikes, a U.S.-based bike-sharing company, has experienced a drop in revenue. To counter this, the company wants to better understand bike demand trends and key influencing factors so they can devise effective strategies to meet customer needs as demand rebounds.
> 
> ### Business Problem:
> The project’s aim is to help BoomBikes predict demand fluctuations more accurately by identifying significant factors that influence bike demand. By understanding these relationships, the company can:
> - Adjust bike supply across different locations,
> - Create targeted marketing campaigns,
> - Optimize maintenance schedules,
> - Improve overall customer satisfaction.
> 
> This insight will allow BoomBikes to meet market demand more effectively, giving it a competitive edge in a potentially recovering market.
> 
> ### Dataset:
> The dataset contains daily bike demand records in the American market, collected based on various factors including meteorological conditions, time of year, and notable calendar events. The dependent variable is the count of daily shared bike rentals (`cnt`), while independent variables include:
> - **Yearly indicators** (`yr`) 
> - **Holiday indicator** (`holiday`)
> - **Temperature** (`temp`)
> - **Humidity** (`hum`)
> - **Windspeed** (`windspeed`)
> - **Seasonal indicators** (e.g., `Summer`, `Winter`)
> - **Monthly indicators** (e.g., `Aug`, `Sep`)
> - **Weather conditions** (`Clear`)
>
>The linear regression model aims to evaluate the significance of each of these variables, allowing the company to quantify their effects on demand.


## Conclusions
> To analyze and deduce conclusions from the multiple linear regression model for predicting the demand for shared bikes, let's break down the insights from each coefficient and how they impact the target variable `cnt` (bike demand). This model is structured as follows:

> `cnt = 0.2075 + (0.2307 * yr) - (0.0897 * holiday) + (0.5378 * temp) - (0.2227 * hum) - (0.2113 * windspeed) + (0.1081 * Summer) + (0.1428 * Winter) + (0.0610 * Aug) + (0.1225 * Sep) + (0.0592 * Clear)`

> ### Interpretations and Business Implications
> 
> 1. **Year (`yr`) - 0.2307**  
>    - Positive impact on demand, indicating an increase in bike usage over the years.
>    - **Business Implication**: This trend can be capitalized on by increasing investment in fleet expansion and marketing as more people adopt bike-sharing services.
> 
> 2. **Holiday (`holiday`) - -0.0897**  
>    - Negative impact, meaning demand slightly decreases on holidays.
>    - **Business Implication**: To counter lower demand on holidays, BoomBikes could offer promotions, such as discounted rates on holidays, to encourage usage.
> 
> 3. **Temperature (`temp`) - 0.5378**  
>    - High positive impact, showing demand significantly increases with temperature.
>    - **Business Implication**: Marketing and maintenance resources should focus on peak seasons with favorable temperatures to maximize profitability and availability of bikes.
> 
> 4. **Humidity (`hum`) - -0.2227**  
>    - Negative impact, indicating higher humidity levels reduce bike demand.
>    - **Business Implication**: In high-humidity periods, promotional efforts could be redirected to offset the drop in demand, possibly through targeted indoor fitness collaborations.
> 
> 5. **Windspeed (`windspeed`) - -0.2113**  
>    - Negative impact, as strong winds reduce bike usage.
>    - **Business Implication**: Given that windier days see lower demand, adjust fleet management to prevent over-deployment in such conditions, thus saving operational costs.
> 
> 6. **Seasonal Variables (Summer, Winter)**  
>    - **Summer (0.1081)** and **Winter (0.1428)** both show positive impacts, with Winter having a slightly higher coefficient.
>    - **Business Implication**: BoomBikes could tailor seasonal marketing strategies, such as winter bike preparedness campaigns or summer leisure biking promotions, to cater to demand shifts during these seasons.
> 
> 7. **Monthly Variables (August, September)**  
>    - **August (0.0610)** and **September (0.1225)** both show positive demand impacts, with September higher than August.
>    - **Business Implication**: These months might represent a seasonal high in demand; additional resources like more bike availability and maintenance crews can ensure service efficiency during peak times.
> 
> 8. **Clear Weather (`Clear`) - 0.0592**  
>    - Positive effect on bike demand, indicating higher usage in clear weather.
>    - **Business Implication**: Market outdoor experiences and activities on clear days to leverage the natural increase in demand.

### Conclusion

> The model provides valuable insights into key factors affecting bike demand:
> 
> - Seasonal and weather-related factors are highly influential. BoomBikes can optimize their inventory and staffing levels according to expected demand fluctuations.
> - By understanding periods of low demand (e.g., windy or high-humidity days), BoomBikes can deploy targeted marketing or promotional campaigns to incentivize users.
> - With temperature and year trends both positively impacting demand, BoomBikes can anticipate growth over time, which is essential for long-term strategic planning.


## Technologies Used
> - **Python** - Version 3.17
> - **Pandas** - Version 2.1.4
> - **NumPy** - Version 1.26.4
> - **Matplotlib** - Version 3.8.0
> - **Seaborn** - Version 0.13.2
> - **Jupyter Notebook** - Version 7.0.8


## Acknowledgements
> - **Data Source**: The day.csv dataset provided for this analysis from UpGrad.
> - **Educational Resources**: Various online resources and courses that helped in learning EDA, Linear Regression.


## Contact
Created by [@sowmilydutta]
