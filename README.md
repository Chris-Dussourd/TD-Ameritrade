# TD-Ameritrade

API to make requests to the TD Ameritrade Site. You need a TD Ameritrade account for this to work.

Steps for Authenticating your App: Go to https://developer.tdameritrade.com/, 

1. Create an app on the developer site
2. Select a callback URL (Ex: localhost)
3. Open the auth_info.py file and fill out information related to your account
    - redirect_uri = your callback url
    - consumer_key = provided by TD Developer site in your app
    - username = TD Ameritrade account (not developer site)
    - password = TD Ameritrade account (not developer site)

4. Run the Authentication.py file
    - A browser will open and login to your TD site. It will ask for two factor authentication. 
    - Once you two factor authenticate, enter 'Done' into the python terminal
    - The refresh token will be printed into the terminal. Copy it to your auth_info file.

TDAmeritrade_API contains the following functions:
  get_access - gets an access token from the site
  get_user_principles - user data used to connect to the websocket
  get_orders - get orders of a particular status using a date range
  get_order_by_id - get a particular order
  delete_order - delete a particular order 
  post_order - place an order
  replace_order - update a particular order
  build_order_request - pass in session, duration, orderType, orderLegCollection, and orderStrategy to create a correctly formatted order request
  get_quote - get a quote by ticker
  get_multi_quotes - get quotes for multiple tickers
  get_price_history_lookback - get the price history using a lookback period (days, months, year, ytd)
  get_price_history_date - use a start and end date to get price history

