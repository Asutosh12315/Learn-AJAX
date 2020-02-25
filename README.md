# AJAX-Corner
## AJAX Fundamental Concepts and Interview Questions Zone


### AJAX Introduction

1. AJAX is an acronym for Asynchronous JavaScript and XML.
2. It is a group of inter-related technologies like JavaScript, DOM, XML, HTML/XHTML, CSS, XMLHttpRequest etc.
3. AJAX allows you to send and receive data asynchronously without reloading the web page. So it is fast.
4. AJAX allows you to send only important information to the server not the entire page. So only valuable data from the client side is routed to the server side. It makes your application interactive and faster.
5. AJAX is not a programming language.

### How AJax Work

[Ajax Work Flow link] (https://github.com/Programming-Interview-Preparation/Learn-AJAX/blob/master/images/ajax.png)


### Understanding Synchronous vs Asynchronous

#### Synchronous (Classic Web-Application Model)
1. A synchronous request blocks the client until operation completes i.e. browser is unresponsive. In such case, javascript engine of the browser is blocked.


[See Image](https://github.com/Programming-Interview-Preparation/Learn-AJAX/blob/master/images/synchronous.gif)

2. As you can see in the above image, full page is refreshed at request time and user is blocked until request completes.

[Let's understand it another way.](https://github.com/Programming-Interview-Preparation/Learn-AJAX/blob/master/images/synchronousrequest.jpg)


#### Asynchronous (AJAX Web-Application Model)
1. An asynchronous request doesn’t block the client i.e. browser is responsive. At that time, user can perform another operations also. In such case, javascript engine of the browser is not blocked.
[See Image ](https://github.com/Programming-Interview-Preparation/Learn-AJAX/blob/master/images/asynchronous.gif)
2. As you can see in the above image, full page is not refreshed at request time and user gets response from the ajax engine. 

[Let's try to understand asynchronous communication by the image.](https://github.com/Programming-Interview-Preparation/Learn-AJAX/blob/master/images/asynchronousrequest.jpg)

### AJAX Technologies
* As describe earlier, ajax is not a technology but group of inter-related technologies. AJAX technologies includes:

1. HTML/XHTML and CSS
2. DOM
3. XML or JSON
4. XMLHttpRequest
5. JavaScript

#### HTML/XHTML and CSS
* These technologies are used for displaying content and style. It is mainly used for presentation.

#### DOM
* It is used for dynamic display and interaction with data.

#### XML or JSON
* For carrying data to and from server. JSON (Javascript Object Notation) is like XML but short and faster than XML.

#### XMLHttpRequest
* For asynchronous communication between client and server.

#### JavaScript
It is used to bring above technologies together. Independently, it is used mainly for client-side validation.

### Understanding XMLHttpRequest
* An object of XMLHttpRequest is used for asynchronous communication between client and server.
* It performs following operations:
1. Sends data from the client in the background
2. Receives the data from the server
3. Updates the webpage without reloading it.

### Properties of XMLHttpRequest object
* The common properties of XMLHttpRequest object are as follows:

| Property        | Description   |
| ------------- |-------------|
| onReadyStateChange      | It is called whenever readystate attribute changes. It must not be used with synchronous requests.|
|readyState	|Represents the state of the request. It ranges from 0 to 4.|
||0 UNOPENED open() is not called.|
||1 OPENED open is called but send() is not called.|
||2 HEADERS_RECEIVED send() is called, and headers and status are available.|
||3 LOADING Downloading data; responseText holds the data.|
||4 DONE The operation is completed fully.|
|reponseText|returns response as text.|
|responseXML|returns response as XML|

### Methods of XMLHttpRequest object
* The important methods of XMLHttpRequest object are as follows:

| Method        | Description   |
| ------------- |-------------|
|void open(method, URL)	| Opens the request specifying get or post method and url.|
|void open(method, URL, async) | Same as above but specifies asynchronous or not.|
|void open(method, URL, async, username, password) |	Same as above but specifies username and password.|
|void send() |	Sends get request.|
|void send(string) |	Send post request.|
|setRequestHeader(header,value)	| It adds request headers.|

### How AJAX works?
* AJAX communicates with the server using XMLHttpRequest object. Let's try to understand the flow of ajax or how ajax works by the image displayed below.

[See Image](https://github.com/Programming-Interview-Preparation/Learn-AJAX/blob/master/images/howajaxworks.png)

* As you can see in the above example, XMLHttpRequest object plays a important role.

1. User sends a request from the UI and a javascript call goes to XMLHttpRequest object.
2. HTTP Request is sent to the server by XMLHttpRequest object.
3. Server interacts with the database using JSP, PHP, Servlet, ASP.net etc.
4. Data is retrieved.
5. Server sends XML data or JSON data to the XMLHttpRequest callback function.
6. HTML and CSS data is displayed on the browser.



##### Learn From:
* [Javatpoint](https://www.javatpoint.com/)
