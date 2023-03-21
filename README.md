# **Web-Development**
--------

## **HTTP Requests and Responses**

### *1.What type of architecture does the HTTP request and response process occur in?*

     The HyperText Transfer Protocol (HTTP) is an application-level protocol


### *2.What are the parts of an HTTP request?*

     The Request Line, REquest Header, And the Request Body


### *3.Which part of an HTTP request is optional?*

     The request Body is Option


### *4.What are the three parts of an HTTP response?*

     Status Line - Describing the massage; Header-containing attributes:Body ,optional-containing data


### *5.Which status-code number class represents errors?*

     400 and 500 one is a client and one is a server


### *6.What are the two most common request methods for a security professional to encounter?*

     Get & Post


### *7.Which type of HTTP request method is used to send data?*

     Post is used to send data.


### *8.Which part of an HTTP request contains the data being sent to the server?*

     The quest body post requested data to the server


### *9.In which part of an HTTP response does the browser receive the web code to generate and style a webpage?*

     The request body data received along with the repsond


## **Using cURL**

###  *10.What are the advantages of using curl over the browser?*

     Ability to manage HTTP requests /Responses in a repeatable, programmatic way
     Ability to quickly HTTP HTTP requests in a way that can be automated
     Allows ability to make adjustments as the security professional work
     Ability to support numerous protocol even if a UI is not present


### *11.Which curl option changes the request method?*

     -X


### *12.Which curl option sets request headers?*

     -H


### *13.Which curl option is used to view the response header?*

     -i


### *14.Which request method might an attacker use to figure out what HTTP requests an HTTP server will accept?*

     options


## **Sessions and Cookies**

###  *15.Which response header sends a cookie to the client?*

     HTTP/1.1 200 OK
     Content-type: text/html
     Set-Cookie: cart=Bob
     Set-cookie is set to cart=bob


### *16.Which request header will continue the client's session?*

     GET /cart HTTP/1.1
     Host: www.example.org
     Cookie: cart=Bob
     The cookie will return the client session



## **Example HTTP Requests and Responses**

### *Use the following sample HTTP request and response to answer the questions in this section:*

### *17.HTTP Request*

     POST /login.php HTTP/1.1
     Host: example.com
     Accept-Encoding: gzip, deflate, br
     Connection: keep-alive
     Content-Type: application/x-www-form-urlencoded
     Content-Length: 34
     Upgrade-Insecure-Requests: 1
     User-Agent: Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.132 Mobile Safari/537.36

     username=Barbara&password=password


 ### *18.What is the request method?*

     The request Method is Post


 ### *19.Which header expresses the client's preference for an encrypted response?*

     Upgrade-Insecure-Requests 1


### *20.Does the request have a user session associated with it?*

     No the session is not restablished yet


 ### *21.What kind of data is being sent from this request body?*

     username=Barbara&password=password


### *23.TTP Response*

     HTTP/1.1 200 OK
     Date: Mon, 16 Mar 2020 17:05:43 GMT
     Last-Modified: Sat, 01 Feb 2020 00:00:00 GMT
     Content-Encoding: gzip
     Expires: Fri, 01 May 2020 00:00:00 GMT
     Server: Apache
     Set-Cookie: SessionID=5
     Content-Type: text/html; charset=UTF-8
     Strict-Transport-Security: max-age=31536000; includeSubDomains
     X-Content-Type: NoSniff
     X-Frame-Options: DENY
     X-XSS-Protection: 1; mode=block

     [page content]


 ### *24.What is the response status code?*

     200 


 ### *25.What web server is handling this HTTP response?*

     Apache webserver


 ### *26.Does this response have a user session associated with it?*

      Set-Cookie: SessionID=5


 ### *27.What kind of content is likely to be in the [page content] response body?*

     text/html


 ### *28.If your class covered security headers, what security request headers have been included?*

     Strict-Transport-Security: max-age=31536000; includeSubDomains
     X-Content-Type: NoSniff
     X-Frame-Options: DENY
     X-XSS-Protection: 1; mode=block




## **Monoliths and Microservices**

### *29.What are the individual components of microservices called?*

     1 Clients 2. Identity Providers 3. API Gateway 4. Messaging Formats 5. Databases 6. Static Content 7. Management 8. Service Discovery


### *30.What is a service that writes to a database and communicates to other services?*

     API


### *31.What type of underlying technology allows for microservices to become scalable and have redundancy?*

     Containers allow for microservcies to be scable and redundant along with load balancers


## **Deploying and Testing a Container Set**

### *32.What tool can you use to deploy multiple containers at once?*

     Docker compose is a tool to deploy multiple container


### *33.What kind of file format is required to deploy a container set?*

     Yaml file


## **Databases**

### *34.Which type of SQL query would you use to view all of the information within a table called customers?*

     Select statements


### *35.Which type of SQL query would you use to enter new data into a table? (You don't need a full query, just the first part of the statement.)*

     Insert into


 ### *36.Why would you never run DELETE FROM <table-name>; by itself?*

     It delete the entire table since it does not have the where clause
