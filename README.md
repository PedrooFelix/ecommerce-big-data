# eCommerce behavior data from multi category store

![](gcpd.gif)

## This dataset contains 67 million users' events from eCommerce website

# How to read it
There are different types of events. See below.

Property | Description
------------ | -------------
event_time | Time when event happened at (in UTC).
event_type | Only one kind of event: purchase.
product_id | ID of a product
category_id | Product's category ID
category_code | Product's category taxonomy (code name) if it was possible to make it. Usually present for meaningful categories and skipped for different kinds of accessories.
brand | Downcased string of brand name. Can be missed.
price | Float price of a product. 
user_id | permanent user ID.

*user_session 	Temporary user's session ID. Same for each user's session. Is changed every time user come back to online store from a long pause.*

## Event types
Events can be:

> view - a user viewed a product
> 
> cart - a user added a product to shopping cart
> 
> remove_from_cart - a user removed a product from shopping cart
> 
> purchase - a user purchased a product
> 
> Multiple purchases per session
> 
> A session can have multiple purchase events. It's ok, because it's a single order.

## Many thanks
Thanks to REES46 Marketing Platform for this dataset.

# Tools:
python
ai notebook in GCP

# Libraries:

```python
import numpy as np # linear algebra
import pandas as pd # data processing, CSV file I/O (e.g. pd.read_csv)
pd.options.display.float_format = "{:,.2f}".format
import seaborn as sns
import matplotlib.pyplot as plt
import matplotlib.dates as mdates
import datetime as dt
import warnings
warnings.simplefilter("ignore")
```
## huge thanks to the steps followed, also good doing the notes : @adilemre

# PRESENTATION IN PREZI:

https://prezi.com/view/hDBtuNflfYB1WtaBNniS/
https://www.youtube.com/watch?v=PCnNCXMYDNg&lc=UgxCSzwC7YvDi7rQQNp4AaABAg
