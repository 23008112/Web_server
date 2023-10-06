# Developing a Simple Webserver

Name: R.Sanjana
Reg No: 23008112
Department:B tech. AI & ML

# AIM:

Develop a webserver to display about top five web application development frameworks.

# DESIGN STEPS:

## Step 1:

HTML content creation is done

## Step 2:

Design of webserver workflow

## Step 3:

Implementation using Python code

## Step 4:

Serving the HTML pages.

## Step 5:

Testing the webserver
# PROGRAM:
Type your code here
```
from http.server import HTTPServer, Base HTTPRequestHandler
content = """  
<html>
<head>
</head>
<body>
<h1>Welcome</h1>
</body>
</html>
"""

class HelloHandler(BaseGTTPRequestHandler):
    def do_GET(self):
    self.send_response(200)
    self.send_header('content-type','text/html;charset=utf-8')
    self.end_headers()
    self.wfile.write(content.encode())

server_address = ('',80)
httpd = HTTPServer(Server_address, HelloHandler)
httpd.server_forever()
 ```

# OUTPUT:
![Alt text](images/webserver1.png)


# RESULT:

The program is executed succesfully
