# Database Structure
##### Database: MySQL
##### Schema Name: PredicSense
##### Details of the table Name
	1>ps_user

		userId (PK)
		userName 
		userLoginId  
		userPassword
		userPhoneNumber
		userEmailId  
		createdDateTime    
		isActive

	#2>ps_web_scraped_data (dataset 4)

		webScrapedId (PK)
		news
		newsWebLink
		createdDate
		isActive

	#3>ps_price_for_scraped_data

		priceForScrapedId (PK)
		price
		createdDate
		isActive

	#4>ps_web_scraped_filter_data (dataset 5)

		webScrapedId (PK)
		news
		createdDate
		isActive

	#5>ps_bar_graph_data (dataset 2)

		barGraphId (PK)
		brokerage_or_analyst 
		stock_name 
		report_date 
		present_price
		target_max 
		target_min
		isActive

	#6>ps_white_space_data

		whiteSpaceId (PK)
		whiteSpaceValue
		userId
		isActive

	#7>ps_user_web_data

		userWebDataId (PK)
		newsId
		upOrDown
		isActive


	#8>ps_twit_mining_data (dataset 6)
	      NA

	#9>dataset 1
	      NA

	#10>dataset 3 
	      NA

## ba.csv

					Stock	askPriceaskSize	bidPricebidSize
	2017-11-20 20:41:27.001304	SPY	0	230	0	0
	2017-11-20 20:41:28.348230	SPY	0	0	0	12
	2017-11-20 20:41:29.776136	SPY	0	230	0	0
	2017-11-20 20:41:31.061887	SPY	0	0	0	220
	2017-11-20 20:41:32.381449	SPY	0	50	0	0


## final_ML.csv
					Stock	mid	REG		SVR		arima	km	LSTM		UD
	2017-11-20 20:20:47.247617	SPY	258.095	258.0950043869	247.2881378022	258.095	258.095	258.0969691086	-2
	2017-11-20 20:20:47.845643	SPY	258.095	258.0950043869	247.2881378022	258.095	258.095	258.0970306432	-2
	2017-11-20 20:20:48.423853	SPY	258.095	258.0950043869	247.2881378022	258.095	258.095	258.0969691086	-2
	2017-11-20 20:20:48.999010	SPY	258.095	258.0950043869	247.2881378022	258.095	258.095	258.09672297	-2


