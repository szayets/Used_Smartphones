### Used_Smartphones
I analyzed the used devices dataset and developed a model to support a dynamic pricing strategy for used and refurbished devices. Additionally, I identified the key factors that significantly influence the price.

#### Business Context
Buying and selling used phones and tablets used to be something that happened on a handful of online marketplace sites. But the used and refurbished device market has grown considerably over the past decade, and a new IDC (International Data Corporation) forecast predicts that the used phone market would be worth $52.7bn by 2023 with a compound annual growth rate (CAGR) of 13.6% from 2018 to 2023. This growth can be attributed to an uptick in demand for used phones and tablets that offer considerable savings compared with new models.

Refurbished and used devices continue to provide cost-effective alternatives to both consumers and businesses that are looking to save money when purchasing one. There are plenty of other benefits associated with the used device market. Used and refurbished devices can be sold with warranties and can also be insured with proof of purchase. Third-party vendors/platforms, such as Verizon, Amazon, etc., provide attractive offers to customers for refurbished devices. Maximizing the longevity of devices through second-hand trade also reduces their environmental impact and helps in recycling and reducing waste. The impact of the COVID-19 outbreak may further boost this segment as consumers cut back on discretionary spending and buy phones and tablets only for immediate needs.

#### Objective
The rising potential of this comparatively under-the-radar market fuels the need for an ML-based solution to develop a dynamic pricing strategy for used and refurbished devices. ReCell, a startup aiming to tap the potential in this market, has hired you as a data scientist. They want you to analyze the data provided and build a linear regression model to predict the price of a used phone/tablet and identify factors that significantly influence it.

#### Data Description
The data contains the different attributes of used/refurbished phones and tablets. The data was collected in the year 2021. The detailed data dictionary is given below.

brand_name: Name of manufacturing brand
os: OS on which the device runs
screen_size: Size of the screen in cm
4g: Whether 4G is available or not
5g: Whether 5G is available or not
main_camera_mp: Resolution of the rear camera in megapixels
selfie_camera_mp: Resolution of the front camera in megapixels
int_memory: Amount of internal memory (ROM) in GB
ram: Amount of RAM in GB
battery: Energy capacity of the device battery in mAh
weight: Weight of the device in grams
release_year: Year when the device model was released
days_used: Number of days the used/refurbished device has been used
normalized_new_price: Normalized price of a new device of the same model in euros
normalized_used_price: Normalized price of the used/refurbished device in euros


#### Installing the libraries with the specified version.
!pip install pandas==2.0.3 numpy==1.25.2 seaborn==0.13.1 matplotlib==3.7.1 scikit-learn==1.2.2 statsmodels==0.14.2


### Actionable Insights and Recommendations
* The model explains approximately 84% of the variation in the data and achieves an accuracy at 4.5% for the normalized used device prices on the test data, indicating good performance of the model.
* An increase of one unit in the main camera megapixels corresponds to a 0.0211 unit increase in the normalized used device prices, assuming all other variables remain constant.
* A one-unit increase in RAM results in a 0.0193 unit increase in the normalized used device prices, with all other variables held constant.
* If the years since release increase by one unit, the normalized used price decreases by 0.0300 units, assuming all other variables are held constant.
* The average normalized used device price is approximately 4.4
* Android OS dominates the dataset, with 93.1% of used devices running on Android.
* Used device prices are highly correlated with new device prices.
* Continue to refine the model and incorporate additional features or data sources to improve predictive accuracy further and better understand market dynamics.
* Maintain stock availability of devices with higher-quality cameras, more RAM, and faster internet connectivity, as these features are associated with higher prices and greater revenue potential.
