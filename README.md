# WeatherApplication
# Run:
node server.js
nodemon server.js
# Server 
NodeJs+Express
npm install --save express
# Client 
EJS (Embedded Javascript). EJS is a templating language.
## Install: 
npm install ejs --save
## Set up: 
app.set('view engine', 'ejs')
# POST Route
We’re going to make use of the body-parser middleware. body-parser allows us to make use of the key-value pairs stored on the req-body object. In this case, we’ll be able to access the city name the user typed in on the client side.
To use body-parser, we must install it first:
npm install body-parser --save
Once installed, we can require it, and then make use of our middleware with the following line of code in our server.js:
const bodyParser = require('body-parser'); // ... // ... app.use(bodyParser.urlencoded({ extended: true }));

# API 
let url = `http://api.openweathermap.org/data/2.5/weather?q=${city}&units=Metric&appid=${apiKey}`
'Metric' for Celsius.
