First, Adding Development Environment Variables In .env is available with react-scripts@0.5.0 and higher. This means u do not have to install anything 😃.
Second create your .env file or .env*developement file or whatever and place ur variable but and this is the big but add REACT_APP* to each variable name for ex REACT*APP_API_KEY= "secret_key_here". Without adding REACT_APP* you will get undefined issue.
Now, You can simply use this variable process.env.REACT_APP_VARIBALE_NAME. for ex: const API_KEY = process.env.REACT_APP_API_KEY.
Finally, we solved this miserable situation 😇.

https://dev.to/jam3/managing-env-variables-for-provisional-builds-h37

https://betterprogramming.pub/managing-environments-for-provisional-builds-with-react-app-1fb411e3597

https://create-react-app.dev/docs/adding-custom-environment-variables

https://create-react-app.dev/docs/advanced-configuration
