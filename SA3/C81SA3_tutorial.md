Create the First Block
======================


In this activity, you will learn to create the First block for the blockchain.




<img src= "https://github.com/procodingclass/tutorial_images/blob/main/C58SA1.gif?raw=true" width = "180" height = "320">




Follow the given steps to complete this activity:
1. Make a request.


* Open file `app.py`.


* Create the dictionary named `blockData` and add the block data to it.


    `blockData = {
  "sender": sender,
  "receiver": receiver,
  "amount": amount
}`


* Send the dictionary to `index.html` file.


    `@app.route("/", methods= ["GET", "POST"])`


* Using `Jinja` combine conditional statements, loops, variables, etc., in HTML:
Use conditional statements to  display the block.
 
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
