# docker-compose-test-environment

A docker-compose configuration for fast setup of production environment.

## usage

Install _Docker_ and _docker-compose_ and run

	docker-compose up


## environment description

	product-details-database	product-prices-database
				|							|
				v							v
	product-details-service		product-prices-service
				  \						  /
				    \					/
				      \				  /
				        \			/
				         v		   v
				     product-offer-service

The `product-offer-service` provides following information:

- http://product-offer-service/offers
- http://product-offer-service/offer?productNumber={1..n}