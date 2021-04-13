#### HTTP is a protocol which allows the fetching of resources, such as HTML documents. It is the foundation of any data exchange on the Web and it is a client-server protocol, which means requests are initiated by the recipient, usually the Web browser. A complete document is reconstructed from the different sub-documents fetched, for instance text, layout description, images, videos, scripts, and more.
![HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview/fetching_a_page.png)
* Clients and servers communicate by exchanging individual messages (as opposed to a stream of data). The messages sent by the client, usually a Web browser, are called requests and the messages sent by the server as an answer are called responses.
![HTTP](https://mdn.mozillademos.org/files/13673/HTTP%20&%20layers.png)

* HTTP is a client-server protocol: requests are sent by one entity, the user-agent (or a proxy on behalf of it). Most of the time the user-agent is a Web browser, but it can be anything, for example a robot that crawls the Web to populate and maintain a search engine index.

Each individual request is sent to a server, which handles it and provides an answer, called the response. Between the client and the server there are numerous entities, collectively called proxies, which perform different operations and act as gateways or caches, for example.

##### An example HTTP request:
We can create an HttpUrlConnection instance using the openConnection() method of the URL class. Note that this method only creates a connection object but doesn't establish the connection yet.

![req](https://cdn.crunchify.com/wp-content/uploads/2013/03/How-to-Send-HTTP-Request-and-Capture-Response-in-Java.png)

#### An example response:
![req](https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview/http_response.png)
An HttpResponse is not created directly, but rather returned as a result of sending an HttpRequest. An HttpResponse is made available when the response status code and headers have been received, and typically after the response body has also been completely received. Whether or not the HttpResponse is made available before the response body has been completely received depends on the BodyHandler provided when sending the HttpRequest.







