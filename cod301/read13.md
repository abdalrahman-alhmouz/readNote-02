# Read: 13 - Update/Delete

## Sending form data 

![image](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data/client-server.png)

### On the client side: defining how to send the data ,
 The two most important attributes are :

 1- action  : The action attribute defines where the data gets sent. Its value must be a valid relative or absolute URL.

 2- method  : The method attribute defines how data is sent , the most common being the GET method and the POST method.

* With a GET request the user will see the data in their URL bar, but with a POST request they won't.
 This can be very important for two reasons:

1. If you need to send a password (or any other sensitive piece of data), never use the GET method or you risk displaying it in the URL bar, which would be very insecure.

2. If you need to send a large amount of data, the POST method is preferred because some browsers limit the sizes of URLs. In addition, many servers limit the length of URLs they accept.

### On the server side: retrieving the data 

Whichever HTTP method you choose, the server receives a string that will be parsed in order to get the data as a list of key/value pairs. The way you access this list depends on the development platform you use and on any specific frameworks you may be using with it.

### Security issues

HTML forms are by far the most common server attack vectors (places where attacks can occur). 
The problems come from how the server handles data.

**How do you fight these threats?**

* Escape potentially dangerous characters :
The specific characters you should be cautious with vary depending on the context in which the data is used and the server platform you employ, but all server-side languages have functions for this.

* Limit the incoming amount of data to allow only what's necessary.

* Sandbox uploaded files :
Store them on a different server and allow access to the file only through a different subdomain or even better through a completely different domain.

