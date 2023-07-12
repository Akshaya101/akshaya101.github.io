---
title: "What are APIs?"
date: 2022-05-23T20:09:54+05:30
description: 'This article summarizes the what are APIs and how are they implemented in JavaScript.'
ShowBreadCrumbs: true
ShowToc: true
TocOpen: false
cover:
    image: "images/apiss.webp"
    # can also paste direct link from external site
    # ex. https://i.ibb.co/K0HVPBd/paper-mod-profilemode.png
    alt: "<alt text>"
    caption: "<text>"
    relative: false # To use relative path for cover image, used in hugo Page-bundles
---
### Introduction to APIs
Application Programming Interface or API is a software intermediatory that allows two or more computers or devices to interact with each other.

You can think of APIs as interfaces between applications and servers that allow requests and responses to be sent and received.

API Architectural Styles
API designing can be described as the process of planning and deciding on the structure of an API during its development. The architectural style for API can be defined as a large-scale, predefined solution structure. Using an architectural style helps us design solutions quicker than designing the API from scratch.

### Different Architectural Styles present are :

- REST API Style
- GraphQL API Style
- SOAP API Style


API calls can be made in 3 ways :

1. XMLHttpRequest

XHR objects are used to interact with the servers. You can retrieve data from a URL without having to do a full page refresh. XHR is used heavily in AJAX Programming.

AJAX stands for Asynchronous JavaScript and XML. It makes use of the XHR object to communicate with the server. It can send and receive information in multiple types like HTML, JSON, XML and text files. In AJAX programming you don't have to refresh the page to update the information.

```javascript
//create an XHR object
const xhr = new XMLHttpRequest()

//Initalizes a request
xhr.open('GET', 'https://jsonplaceholder.typicode.com/posts', true)
//sends a request
xhr.send()
//fires an XHR transaction
xhr.onload = () => {
    if (xhr.status == 200) {
        console.log(JSON.parse(xhr.response))
    }
    else {
        console.log(xhr.status + ' error occurred!')
    }
}
```
XHR gives a response as a String, so it has to be converted to JSON.

Before ES6 came out, XHR was the only way to make an HTTP request. It is a built-in object with the browser and allows you to make an HTTP request. This was deprecated in ES6 when fetch was introduced.

2. Fetch API

Fetch provides a generic definition of Request and Response objects. This will allow them to be used wherever they are required in future.

The fetch() method takes one argument, which is the resource whose data has to be fetched.

- The fetch method takes in the resource you want to fetch and returns a promise that resolves the Response object.
- This response object does not contain an actual JSON response body but it is a representation of the entire HTTP response,
- So to get the JSON body content from the response object we use the .json() method.
- By doing the above we are trying to achieve the response from the fetch method in the form of a JSON object.

```
//using the fetch() method

fetch('https://jsonplaceholder.typicode.com/posts')
    //this step is responsible for resolving Promise received into JSON
    .then(response => {
        return response.json()
    })
    .then(data => {
        console.log(data)
    })
    .catch(err => {
        console.log(err)
    })
```

3. Axios

Axios is a Promise-based HTTP Client for the browser and Node.js. It can run on the browser as well as within Node.js (making Axios isomorphic in nature).

On the server-side, Node.js uses the Native HTTP modules, on the client-side, browser uses its XMLHttpRequests.
Axios requires you to add CDN if you are trying to implement it on the browser or installation if you are trying to implement it using Node.js.
```javascript
//using axios in Node.js env
const axios = require('axios')

axios('https://jsonplaceholder.typicode.com/posts')
    .then(response => {
        console.log(response.data)
    })
```

### Importance of APIs

- APIs are great time savers, they save you from repetetive workFor instance, consider you have to sign-in into a bunch of website, all you have to do is provide your Gmail credentials, where all the heavy lifiting of authentication is taken care of by Gmail.
- Play an important role in building data drive applicationsAPIs allow the line of business users and IT to leverage software and applications to increase productivity and improve the bottom line.
- APIs play a very important role not only from a technical standpoint but also from a business standpoint. Having APIs available openly for people to use increases revenue for the company, integrating with other applications and gain popularity for the product amongst the community. It also provides a chance for technical innovation to add value to the product itself.