# 4_3_1 Fetch

## Task 1a

Create a web page that displays random dad jokes. You can get your dad jokes from https://icanhazdadjoke.com/ using fetch. (API documentation can be found here: https://icanhazdadjoke.com/api )

## Task 1b

Create a refresh button that requests a new dad joke from the server, and once the response is returned, displays it.

## Task 1c (stretch)

Use some nice CSS transitions to show new facts. Inspiration: https://theuselessweb.site/niceonedad/ (Länkar till en externa sida.)

## Task 2

For this task, you will need to run your own small server. I have made it for you. All you need to do is clone the repo from https://github.com/thomasbrunstrom/academy-proxy-server and run `npm install` and `npm start`

Create a string reverse tool. The user should input a string in a form. The value of the input should be sent to http://127.0.0.1:5050/reverse as a POST request with a JSON payload (body). The response will contain a new json string that you should parse and display.

The server expects the request body to look like this: { "message": "string to be reversed" }.

## Task 3

Using the same server as you were running in task 2, create a XKCD viewer. You have two endpoints http://127.0.0.1:5050/xkcd and http://127.0.0.1/xkcd/{id} These endpoints return the latest XKCD comic, or a XKCD comic with a specific ID. Use the endpoints to create your own nice xkcd viewer in HTML / CSS and JS. The real deal is found here for inspiration: xkcd.com.

## Task 4

Create a form for food order with input for first name, last name, age and allergy preferences. In addition to a checkbox list for food (burger, pizza, hot dogs). On submit, a POST request should be sent to http://127.0.0.1:5050/echo with the details from the form as JSON. The endpoint will return the same data you send in to it (given that it is JSON). So once you get the response, display the receipt for the food order in a nice way in the browser.
