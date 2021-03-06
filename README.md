# Predict Future Sales

COMP9417 Project Repository by Zixin Zhou (Cindy) and Sophia Tran

## Overview
Predicting total sales for every product and store in the next month using different ML algorithms

**input** - daily historical sales data and a test set
(*Note: list of shops and products slightly changes every month*)

**output** - total amount of products sold in every shop for the test set

## Data
### File descriptions:
- **sales_train.csv** - the training set. Daily historical data from January 2013 to October 2015.
- **test.csv** - the test set. You need to forecast the sales for these shops and products for November 2015.
- **sample_submission.csv** - a sample submission file in the correct format.
- **items.csv** - supplemental information about the items/products.
- **item_categories.csv**  - supplemental information about the items categories.
- **shops.csv** - supplemental information about the shops.

### Files:
#### sales_train.csv
| varaible name | description |
| ------------- | ----------- |
| date | date in format dd/mm/yyyy|
| date_block_num | a consecutive month number, used for convenience. January 2013 is 0, February 2013 is 1,..., October 2015 is 33 |
| shop_id | unique identifier of a shop |
| item_id | unique identifier of a product |
| item_price | current price of an item |
| item_cnt_day | number of products sold. You are predicting a monthly amount of this measure |

#### test.csv
| varaible name | description |
| ------------- | ----------- |
| ID | an Id that represents a (Shop, Item) tuple within the test set |
| shop_id | unique identifier of a shop |
| item_id | unique identifier of a product |

#### sample_submission.csv
| varaible name | description |
| ------------- | ----------- |
| ID | an Id that represents a (Shop, Item) tuple within the test set |
| item_cnt_day | number of products sold. You are predicting a monthly amount of this measure |

#### items.csv
| varaible name | description |
| ------------- | ----------- |
| item_name | name of item |
| item_id | unique identifier of a product |
| item_category_id | unique identifier of item category |

#### item_categories.csv
| varaible name | description |
| ------------- | ----------- |
| item_category_name | name of item category |
| item_category_id | unique identifier of item category |

#### shops.csv
| varaible name | description |
| ------------- | ----------- |
| shop_name | name of shop |
| shop_id | unique identifier of a shop |

lstm score: 1.02012
conv score: 1.13260
linear score: