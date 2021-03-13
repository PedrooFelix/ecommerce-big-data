# eCommerce behavior data from multi category store

![](gcpd.gif)

## This dataset contains 67 million users' events from eCommerce website

# How to read it
There are different types of events. See below.

Property | Description
------------ | -------------
Content cell 1 | Content cell 2
event_time | Time when event happened at (in UTC).
event_type | Only one kind of event: purchase.
product_id | ID of a product
category_id | Product's category ID
category_code | Product's category taxonomy (code name) if it was possible to make it. Usually present for meaningful categories and skipped for different kinds of accessories.
brand | Downcased string of brand name. Can be missed.
price | Float price of a product. 
user_id | permanent user ID.

* user_session**	Temporary user's session ID. Same for each user's session. Is changed every time user come back to online store from a long pause. *




#tools used 
python

# in gcp

# PRESENTATION:

https://prezi.com/view/hDBtuNflfYB1WtaBNniS/
