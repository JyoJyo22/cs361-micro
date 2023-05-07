
## CS 361:    Microservice

Author:    Joseph Houghton     <br>
Partner:   Myles Penner        <br>

---

#### General:
This is a microservice which takes in a name of a location and returns details on that location which can be used for   <br>
many purposes. In this case, my partner's front-end app will be sending in the name of a beach and this microservice  <br>
responds with these details which include geographic coordinates, and these coordinates will be used to generate weather    <br>
data (in the front-end app) for the given beach supplied by the user. This microservice is implemented as an Express.js    <br>
Rest API. The details of the request and the response can be seen below.   <br>

---

#### How to Request:    
A front-end app needs to send an HTTP Get request in order to access this microservice endpoint. This HTTP request    <br>
will need to be in the form of:   "server/get/beachname"   where "server" is the name of the server that is hosting    <br>
this microservice, and where "beachname" is the name of the beach that the user wishes to receive data on. An example    <br>
of the code to accomplish this request (using the fetch API) can be seen in the UML diagram below. Later in the     <br>
implementation/integration of this microservice, the hosting site render.com will be used to host this microservice.    <br>
                     
---    
    
#### How to Receive:    
The HTTP response will be received through the same HTTP Get request that the user sends from the front-end app. The    <br>
user simply has to store the result of their Get request into a variable and that variable will contain the data on     <br>
the desired beach that they sent the name of. The user can utilize the "async" and "await" keywords of Javascript in    <br>
order to wait for the Javascript "promise" to be fulfilled before they try to access/use the data they receive back.    <br>
An example of the code which sends back this response can be seen in the UML diagram below.    <br>

---

![Image](https://github.com/JyoJyo22/cs361-micro/blob/master/cs361-assign8-UML.png)

