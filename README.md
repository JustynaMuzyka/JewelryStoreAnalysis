# Contents
* [Dataset overview](#dataset-overview)
* [Dataset analysis](#dataset-analysis)
* [Used libraries and packages](#used-libraries-and-packages)

# Dataset overview
## Metadata after cleansing
|   Column      | Non-Null Count |        Dtype       |
| --------------|----------------|--------------------|
| date          |      80625     | datetime64[ns, UTC]|
| order_id      |      80625     |       int64        | 
| product_id    |      80625     |       int64        |
| category      |      80625     |       object       |
| brand_id      |      77120     |       float64      |
| price         |      80625     |       float64      |
| user_id       |      80625     |       float64      |
| main_color    |      78390     |       object       |
| main_metal    |      80533     |       object       |
| main_gem      |      61007     |       object       |

dtypes: datetime64[ns, UTC](1), float64(3), int64(2), object(4)
memory usage: 6.2+ MB

## Reference
https://www.kaggle.com/mkechinov/ecommerce-purchase-history-from-jewelry-store

# Dataset analysis
In order to provide valuable analysis I prepared:
* Summary revenue from various product categories.
* Various product categories selling details over the time.

In order to predict future store income I used polynomial regression.
To predict future sales of specific product categories, I used time series forecasting.

# Used libraries and packages
* numpy 
* pandas 
* matplotlib 
* seaborn 
* tensorflow
* pyplot
* polyfit
