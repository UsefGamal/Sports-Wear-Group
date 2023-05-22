# Sports-Wear-Group
## Objective And Problem Statement

## Focus Of Analytics Project :
- marketing team will be interest to see if they can `increase their efficiency`
- the management team want to know if using advanced analytics may `increase sales` in general.

 Attributes:
- `country`:	Country name
- `article`: 	6 digit article number, as unique identifier of an article
- `sales`: 		total number of units sold in respective retail week
- `regular_price` : 	recommended retail price of the article
- `current_price` :  current selling price (weighted average over the week)
- `ratio` : 		price ratio as current_price/regular_price, such that price discount is 1-ratio 
- `retailweek` : 	start date of the retailweek
- `promo1` : 	indicator for media advertisement, taking 1 in weeks of activation and 0 otherwise
- `promo2` : 	indicator for store events, taking 1 in weeks with events and 0 otherwise
- `customer_id` : 	customer unique identifier, one id per customer
- `article` :  	6 digit article number, as unique identifier of an article
- `productgroup` : 	product group the article belongs to
- `category` : 	product category the article belongs to
- `cost` : 		total costs of the article (assumed to be fixed over time)
- `style` : 		description of article design
- `sizes` : 		size range in which article is available
- `gender` : 	gender of target consumer of the article
- `rgb_*_main_color`:	intensity of the red (r), green (g), and blue (b) primaries of the article‘s  main color, 		taking values [0,250]
- `rgb_*_sec_color`:	intensity of the red (r), green (g), and blue (b) primaries of the article‘s secondary 		color, taking values [0,250]
- `label`:		advertisement result after offering/sending/presenting the offer to the customer. 0 means the customer did not buy and 1 means the costumer did buy.

## Description
- ```article``` 477 distinct values	High ```cardinality```
- ```retailweek``` 123 distinct Weeks	High ```cardinality```
- ```regular_price``` is highly overall correlated with current_price	High ```correlation```
- ```current_price``` is highly overall correlated with regular_price	High ```correlation```
- ```productgroup``` is highly overall correlated with cost 	High ```correlation```
- ```category``` is highly overall correlated with cost 	High ```correlation```
- ```style``` is highly overall correlated with cost 	High ```correlation```
- ```sizes``` is highly overall correlated with cost 	High ```correlation```
- ```gender``` is highly overall correlated with cost 	High ```correlation```
- ```closest_colors_main``` is highly overall correlated with cost 	High ```correlation```
- ```closest_colors_sec``` is highly overall correlated with cost 	High ```correlation```
- ```promo1``` is highly imbalanced (66.5%)	```Imbalance```
- ```promo2``` is highly imbalanced (95.5%)	```Imbalance```
- ```sizes``` is highly imbalanced (53.1%)	```Imbalance```
- ```article```.1 is uniformly distributed	```Uniform```
