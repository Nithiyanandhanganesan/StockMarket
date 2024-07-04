Alpaca has 4 API options
========================

  - Broker API : 
         If you are building trading apps.
  - Trading API: 
        If you doing algorithmic trading.
  - Market Data API:
        Access real-time market pricing data and up to 6+ years worth of historical data for stocks and crypto.
  - Connect API : 
        Develop applications on Alpaca’s platform using OAuth2.  
        Let any user with an Alpaca brokerage account connect to your app.

Official Client SDKs:
=====================
 - Python: alpaca-py / PyPI
 - Node: alpaca-trade-api-js / npm
 - Go: alpaca-trade-api-go
 - Python (legacy): alpaca-trade-api-python / PyPI

Trading API:
==============
 - Paper trading is free and available to all Alpaca users.
 - Alpaca also offers live brokerage accounts (with real money) for individuals and businesses plus crypto accounts.
 - Alpaca offers crypto trading through our API and the Alpaca web dashboard!
 - Our Trading API supports different order types such as market, limit and stop orders plus more complex ones.
 - You can Buy Fractional Shares as well.
 - In the Paper environment, options trading capability will be enabled by default - there's nothing you need to do!

API:
----
Alpaca’s live API domain is https://api.alpaca.markets
Alpaca's Paper trading domain is https://paper-api.alpaca.markets.

curl -X GET \
-H "APCA-API-KEY-ID: {YOUR_API_KEY_ID}"  
-H "APCA-API-SECRET-KEY: {YOUR_API_SECRET_KEY}"  
https://{apiserver_domain}/v2/account

Alpaca’s paper trading service uses a different domain and different credentials from the live API. 
You’ll need to connect to the right domain so that you don’t run your paper trading algo on your live account.


CAll this API to get the request id:
curl -v https://paper-api.alpaca.markets/v2/account

In the response , you can find X-Request-ID.






