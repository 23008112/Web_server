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
Top Five Web Development Frameworks
</head>
<body>
<h1>Welcome</h1>
1. Diango

2.MEAN Stack

3.React
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
![Alt text](images/webserver.jpg)


![webserver1](https://github.com/23008112/Web_server/assets/138972470/48d67a0e-9ef1-4ec1-a5c8-79762e07833d)

# RESULT:

The program is executed succesfully
