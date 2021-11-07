# PD_01
In this project we were asked to analyse data from an online Store collected over 4 months (April - July 2014). Three files with the datasets to be used in pattern mining were provided.

The file store-buys.dat comprises the buy events of the users over the items. It contains 318.444 sessions. Each record/line in the file has the following fields (with this order):

    Session ID - the id of the session. In one session there are one or many buying events. Could be represented as an integer number.
    Timestamp - the time when the buy occurred. Format of YYYY-MM-DDThh:mm:ss.SSSZ
    Item ID – the unique identifier of item that has been bought. Could be represented as an integer number.
    Price – the price of the item. Could be represented as an integer number.
    Quantity – the quantity in this buying. Could be represented as an integer number.

The file store-clicks.dat comprises the clicks of the users over the items. It contains 5.613.499 sessions. Each record/line in the file has the following fields (with this order):

    Session ID – the id of the session. In one session there are one or many clicks. Could be represented as an integer number.
    Timestamp – the time when the click occurred. Format of YYYY-MM-DDThh:mm:ss.SSSZ
    Item ID – the unique identifier of the item that has been clicked. Could be represented as an integer number.
    Context – the context of the click. The value "S" indicates a special offer, "0" indicates a missing value, a number between 1 to 12 indicates a real category identifier, any other number indicates a brand. E.g. if an item has been clicked in the context of a promotion or special offer then the value will be "S", if the context was a brand i.e BOSCH, then the value will be an 8-10 digits number. If the item has been clicked under regular category, i.e. sport, then the value will be a number between 1 to 12.

The file products.csv comprises the list of products sold by the online store. It contains 46.294 different products associated with 123 different subcategories. Each record/line in the file has the following fields:

    Item ID - the unique identifier of the item. Could be represented as an integer number.
    Product Categories - the category and subcategories of the item. It is a string containing the category and subcategories of the item. Eg. appliances.kitchen.juice

In this project we used Python 3, Jupyter Notebook and MLxtend. When using MLxtend, frequent patterns were discovered using FP-Growth.
