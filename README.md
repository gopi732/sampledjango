Assignment Content

In this lab, you will develop a simple Hello World Django app. The app consists of one route and returns a JSON object with a Hello World message.



Response JSON should look like below:



{“Message”: “Hello World!”}



Create a git repo in GitHub, and push your entire Django project directory into GitHub, also, make sure to include a README file describing how to run/start your web app and how to access the Hello World JSON response in a browser.



For submission, click on the Submission text area and add the GIT REPO URL.

https://github.com/gopi732/sampledjango

In conclusion, you have successfully developed a simple Hello World Django app that returns a JSON response and includes an optional HTML template. The app consists of a single route that, when accessed, returns a JSON object with the message "Hello World!".
You followed the steps to create a new Django project, including setting up a Django app, defining the route and view, configuring the project settings, and optionally creating an HTML template. You tested the app by running the Django development server and accessing the JSON response and, if applicable, the HTML template in a browser.
Furthermore, you set up a Git repository on GitHub and pushed the entire Django project, including a README file describing how to run/start the web app and access the Hello World JSON response, to the repository.


Optional Challenge:

To render a simple HTML page with a message formatted in bold, you can create a Django template and modify the view to render this template.

Step 1: Create a Template

Inside the HelloWorldApp directory, create a folder called templates.
Inside templates, create a new file named hello.html.

Step 2: Write HTML Template

In hello.html, write the HTML code to display the "Hello World!" message in bold:

<!DOCTYPE html>
<html>
<head>
    <title>Hello World Page</title>
</head>
<body>
    <h1>Hello World!</h1>
    <p><strong>This is bold text!</strong></p>
</body>
</html>

Step 3: Modify the View
Update the views.py file in your Django app to render this template:

from django.shortcuts import render

def hello_world(request):
    return render(request, 'hello.html')
Step 4: URL Mapping
Make sure the URL mapping in HelloWorldApp/urls.py remains the same as before.

Step 5: Run the Server
Start the Django development server:

python manage.py runserver


Step 6: Access the Rendered HTML Page
Navigate to http://127.0.0.1:8000/hello/ in your browser. You should see the "Hello World!" message displayed in bold text according to the HTML template you created.

This modification in the view's response will render the hello.html template and return the resulting HTML document to the browser.

If you then want to push these changes to your GitHub repository, follow the same steps as mentioned earlier, ensuring your updated code and template files are included.
