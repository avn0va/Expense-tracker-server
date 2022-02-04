# Expense Tracker V2
# [Preview found here](http://skoti.ddns.net:8888)

## Installation

In the "expense-tracker-full" directory in terminal

### Backend installation

Install npm for the project backend
```
npm install
```
Install dependencies
```
npm install colors dotenv express mongoose morgan
```
Install dev dependencies
```
npm install -D concurrently nodemon
```

### Client installation

Install npm for the project client
Go to the client sub directory in the "expense-tracker-full" direcotry
```
cd client
```
And install npm  for the client
```
npm install
```

Install dependencies
```
npm install axios
```


#### NOTE BOTH CLIENT & BACKEND INSTALLATIONS ARE NEEDED FOR THE FULLSTACK APP


## Deploy for production
(Please note this requires npm installation for both client & server)

### Build the client

In the expense-tracker-full/client directory
```
npm run build
```
Go back to root
```
cd ..
```

### Run the server in production mode

Set the project to production mode

In the config/config.env file
``` env
Line 1: NODE_ENV=production 
```
Finally run the application

In the expense-tracker-full directory
```
node server
```
The application should now be running on port 3000 on localhost <br>
Open the application in your browser <br>
http://localhost:3000

## Run the project in developement mode
(Please note we're again assuming you've installed both back- & frontend)

Set the project to development mode

In the config/config.env file
``` env
Line 1: NODE_ENV=development 
```
Open two separate terminal windows

In the expense-tracker-full folder

```
nodemon server
```

In the expense-tracker-full/client folder
```
npm start
```

<b>Keep the terminal windows open in order for the server to keep running</b>

The application should now be running on port 3000 on localhost <br>
Open the application in your browser <br>
http://localhost:3000
