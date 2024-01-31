Sure, here is the design for a Flask application to solve the problem you described:

## Flask Application Design

### HTML Files

**1. index.html:**
   - This will be the home page of the application.
   - It will contain a form to accept user input and submit it to the server.
   - The form will have two fields: "Enter a number" and a "Submit" button.

**2. result.html:**
   - This HTML file will display the result of the user's input.
   - It will contain a heading to display the message "Result" and a paragraph to display the actual result.

### Routes

**1. @app.route('/', methods=['GET', 'POST']):**
   - This route will handle both GET and POST requests to the root URL ('/').
   - When a GET request is made, it will render the `index.html` file, displaying the form.
   - When a POST request is made, it will receive the user input from the form and store it in a variable.
   - It will then pass the value to a function that performs the necessary calculations and returns the result.
   - Finally, it will render the `result.html` file, displaying the calculated result.

**2. @app.route('/calculate', methods=['POST']):**
   - This route will handle POST requests to the '/calculate' URL.
   - When a POST request is made to this URL, it will receive the user input from the form on the `index.html` page.
   - It will then pass the value to a function that performs the necessary calculations and returns the result.
   - Finally, it will redirect the user to the root URL ('/') and display the result in the `result.html` page.

Please note that the functions to perform the necessary calculations and the CSS file for styling are not included in this design, as they are specific to your problem and its solution. However, you can easily add them to your Flask application to make it fully functional.

I hope this design is helpful for you in building your Flask application. Feel free to ask me any further questions you may have.