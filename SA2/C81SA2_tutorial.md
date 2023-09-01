Send Data to Server
===================


In this activity, you will learn to send the data from the HTML page to the server.




<img src= "https://github.com/procodingclass/tutorial_images/blob/main/C58SA1.gif?raw=true" width = "180" height = "320">




Follow the given steps to complete this activity:
1. Make a request.


* Open file app.py.


* Import `render_template and request` from `flask` to render the html page and send http requests.


    `from flask import Flask, render_template, request`


* Add the `GET` and `POST` methods to the route.


    `@app.route("/", methods= ["GET", "POST"])`


* Display the index page if the `request.method` is `GET`.
 
    `if request.method == "GET":
        return render_template('index.html')`


* Add an else condition to get the data that the user entered on the form and send it to the server.


    else:
        sender = request.form.get("sender")
        receiver = request.form.get("receiver")
        amount = request.form.get("amount")


* Print the data on the console and display the index page.


    `print(sender, receiver, amount)`


    `return render_template('index.html')`
   


* Save and run the code to check the output.