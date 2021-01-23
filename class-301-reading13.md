# Sending form data

## Client/server architecture

- At most basic the web uses a client/server articture

- A web client (usually a browser) sends a request to a server, usually (Apache, Nginx, IIS, Tomcat, etc)

- The above communication takes place thanks to HTTP protocol.  The server answers the request with the same protocol.

> An HTML form on a web page is nothing more than a convenient user-friendly way to configure an HTTP request to send data to a server. This enables the user to provide information to be delivered in the HTTP request.

- On the client side: defining how to send the data

- The form element defines how the data will be sent

* All of its attributes are designed to let you configure the request to be sent when a user hits a submit button. The two most important attributes are action and method.

### The action attribute

> The action attribute defines where the data gets sent. Its value must be a valid relative or absolute URL. If this attribute isn't provided, the data will be sent to the URL of the page containing the form — the current page.

> It's possible to specify a URL that uses the HTTPS (secure HTTP) protocol. When you do this, the data is encrypted along with the rest of the request, even if the form itself is hosted on an insecure page accessed using HTTP. On the other hand, if the form is hosted on a secure page but you specify an insecure HTTP URL with the action attribute, all browsers display a security warning to the user each time they try to send data because the data will not be encrypted.

- It's possible to specify a URL that uses the HTTPS (secure HTTP) protocol.

- The action value should be a file on the server that can handle the incoming data, including ensuring server-side validation. The server then responds, generally handling the data and loading the URL defined by the action attribute, causing a new page load (or a refresh of the existing page, if the action points to the same page).

### How the data is sent depends on the method attribute.

- HTML form data can be transmitted via a number of different methods, the most common being the GET method and the POST method

- The browser sends a request to a URL

* An HTTP request consists of two parts: 
- A header that contains a set of global metadata about the browser's capabilities. 
- A body that can contain information necessary for the server to process the specific request.

### The GET method

- Used by the browser to ask the server to send back a given resource.
*Because/If the body is empty, if a form is sent using this method the data sent to the server is appended to the URL.

- After the URL web address has ended, we include a question mark (?) followed by the name/value pairs/each one separated by an ampersand (&)

- we concatenate the value of the value attribute


* Say, which has a value of Hi
to, which has a value of Mom
The HTTP request looks like this:
GET /?say=Hi&to=Mom HTTP/2.0
Host: foo.com

### The POST method

> The POST method is a little different. It's the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request: "Hey server, take a look at this data and send me back an appropriate result." If a form is sent using this method, the data is appended to the body of the HTTP request.

-  If a form is sent using this method, the data is appended to the body of the HTTP request.

- HTTP requests are never displayed to the user (if you want to see them, you need to use tools such as the Firefox Network Monitor or the Chrome Developer Tools)

- Whichever HTTP method you choose, the server receives a string that will be parsed in order to get the data as a list of key/value pairs. 

- The way you access this list depends on the development platform you use and on any specific frameworks you may be using with it.



#### POST VS GET

- If you need to send a password (or any other sensitive piece of data), never use the GET method or you risk displaying it in the URL bar, which would be very insecure.
- If you need to send a large amount of data, the POST method is preferred because some browsers limit the sizes of URLs. In addition, many servers limit the length of URLs they accept.

> This example won't work when you load it into a browser locally — browsers cannnot interpret PHP code, so when the form is submitted the browser will just offer to download the PHP file for you. To get it to work, you need to run the example through a PHP server of some kind. Good options for local PHP testing are MAMP (Mac and Windows) and AMPPS (Mac, Windows, Linux).

> There are many other server-side technologies you can use for form handling, including 

* Perl
* Java
* .Net
* Ruby

- Its god to try them and pick which one best fits your project. These technologies can be hard to use by themselves so it's recommended to use a frakework to help achieve your goals. These great frameworks can make handling forms easier:

- Django for Python (a bit more heavyweight than Flask, but with more  tools and options).
- Express for Node.js.
- Laravel for PHP.
- Ruby On Rails for Ruby.


Reference: https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data
Reference: 