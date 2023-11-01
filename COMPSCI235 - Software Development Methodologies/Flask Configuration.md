[[Flask]] defines several configuration variables
- The settings for these variables influence [[Flask]]'s run-time behaviour

Key environment variables include:
- `FLASK_APP` - where this app is going to start
	- Specifies the app to run when issuing a '`flask run`' command from the terminal
- FLASK_ENV - what environment we want to run at the moment
	- Set to either 'development' or 'production'
		- 'development', switches on debugging mode - which is very useful when developing an app
		- Debugging mode causes:
			- Any exceptions raised to be displayed