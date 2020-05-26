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
