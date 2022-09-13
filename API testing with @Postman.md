
This blog is heavily inspired from the Devtown x Postman workshop led by @ialimustufa .

# What is Postman?

Postman is an API platform for developers to design, build, test and iterate their APIs. As of April 2022, Postman reports having more than 20 million registered users and 75,000 open APIs, which it says constitutes the world's largest public API hub. The company is headquartered in San Francisco and maintains an office in Bangalore, where it was founded.

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/jiqbtj2197fjz30wgtay.png)

Now you might be asking what exactly is an API?Let me tell you in brief what is an API why exactly we use them.

# All About APIs

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/3g1zedsq4x9l8llxqy8l.png)

## What is an API?

**APIs are mechanisms that enable two software components to communicate with each other using a set of definitions and protocols.** For example, the weather bureau’s software system contains daily weather data. The weather app on your phone “talks” to this system via APIs and shows you daily weather updates on your phone.

## What does API stand for?

API stands for `Application Programming Interface`. In the context of APIs, the word Application refers to any software with a distinct function. Interface can be thought of as a contract of service between two applications. This contract defines how the two communicate with each other using requests and responses. Their API documentation contains information on how developers are to structure those requests and responses.

## How do APIs work?

API architecture is usually explained in terms of client and server. The application sending the request is called the client, and the application sending the response is called the server. So in the weather example, the bureau’s weather database is the server, and the mobile app is the client.

**There are four different ways that APIs can work depending on when and why they were created.**

- ### SOAP APIs

    These APIs use Simple Object Access Protocol. Client and server exchange messages using XML. This is a less flexible API that was more popular in the past.

- ### RPC APIs

    These APIs are called Remote Procedure Calls. The client completes a function (or procedure) on the server, and the server sends the output back to the client.

- ### Websocket APIs

    Websocket API is another modern web API development that uses JSON objects to pass data. A WebSocket API supports two-way communication between client apps and the server. The server can send callback messages to connected clients, making it more efficient than REST API.

- ### REST APIs

    These are the most popular and flexible APIs found on the web today. The client sends requests to the server as data. The server uses this client input to start internal functions and returns output data back to the client.

**Let’s look at REST APIs in more detail below.**

## What are REST APIs?

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/y0i4chc9nm9xu3cjtvkg.png)

REST stands for `Representational State Transfer`. REST defines a set of functions like GET, PUT, DELETE, etc. that clients can use to access server data. Clients and servers exchange data using HTTP.

The main feature of REST API is `statelessness`. Statelessness means that servers do not save client data between requests. Client requests to the server are similar to URLs you type in your browser to visit a website. The response from the server is plain data, without the typical graphical rendering of a web page.

## What is web API?

A Web API or Web Service API is an application processing interface between a web server and web browser. All web services are APIs but not all APIs are web services. REST API is a special type of Web API that uses the standard architectural style explained above.

The different terms around APIs, like Java API or service APIs, exist because historically, APIs were created before the world wide web. Modern web APIs are REST APIs and the terms can be used interchangeably.

## What are API integrations?

API integrations are software components that automatically update data between clients and servers. Some examples of API integrations are when automatic data sync to the cloud from your phone image gallery, or the time and date automatically sync on your laptop when you travel to another time zone. Enterprises can also use them to efficiently automate many system functions.

## What are the benefits of REST APIs?

**REST APIs offer four main benefits:**

1. **Integration**

    APIs are used to integrate new applications with existing software systems. This increases development speed because each functionality doesn’t have to be written from scratch. You can use APIs to leverage existing code.

2. **Innovation**

    Entire industries can change with the arrival of a new app. Businesses need to respond quickly and support the rapid deployment of innovative services. They can do this by making changes at the API level without having to re-write the whole code.

3. **Expansion**

    APIs present a unique opportunity for businesses to meet their clients’ needs across different platforms. For example, maps API allows map information integration via websites, Android,iOS, etc. Any business can give similar access to their internal databases by using free or paid APIs.

4. **Ease of maintenance**

    The API acts as a gateway between two systems. Each system is obliged to make internal changes so that the API is not impacted. This way, any future code changes by one party do not impact the other party.

## HTTP Methods used in RESTful API Development

In HTTP there are five methods that are commonly used in a REST-based Architecture i.e., `POST, GET, PUT, and DELETE`. These correspond to create, read, update, and delete (or CRUD) operations respectively. There are other methods which are less frequently used like OPTIONS and HEAD.

1. ### GET Method

    The HTTP GET method is used to read (or retrieve) a representation of a resource. In the safe path, GET returns a representation in XML or JSON and an HTTP response code of `200 (OK)`. In an error case, it most often returns a `404 (NOT FOUND)` or `400 (BAD REQUEST)`.

    ![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/7jev0850iba7dn10hswl.png)

2. ### POST Method

    The POST verb is most often utilized to create new resources. In particular, it’s used to create subordinate resources. That is, subordinate to some other (e.g. parent) resource. On successful creation, return `HTTP status 201`, returning a Location header with a link to the newly-created resource with the 201 HTTP status.

    ![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/8fjzlzgcfbi80ne09jvm.png)

3. ### PUT Method

    It is used for updating the capabilities. However, PUT can also be used to create a resource in the case where the resource ID is chosen by the client instead of by the server. In other words, if the PUT is to a URI that contains the value of a non-existent resource ID. On successful update, return `200` (or `204` if not returning any content in the body) from a PUT. If using PUT for create, return HTTP status 201 on successful creation. PUT is not safe operation but it’s idempotent.

    ![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ao59y53vw2880zhihd43.png)

4. ### DELETE Method

    It is used to delete a resource identified by a URI. On successful deletion, return `HTTP status 200 (OK)` along with a response body.

    ![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/rartkv426m3gl46hx60p.png)

With this I am ending the brief overview about APIs and HTTP methods and about Postman. I hope that you might takeaway something from this blog and implement it in your work.

Special thanks to @ialimustufa , Devtown and Postman Student Committee for organizing such an informative workshop on APIs and Postman.
