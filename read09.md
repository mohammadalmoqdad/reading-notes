

## How does route prefixing work with an external routing module?
that is done by rewuiring that route and use it as importing any other file


## When routing, what’s the difference between app.get('/data/:id') and app.get('/data/:name')?
the one with name will return back the records that has the same name in the url
but with the id it will return the ones whose id match ithe n the url but it would be one record because the id is unique and the name mwy be repeated

## Explain how Express handles routing conflicts?
by using .Router() which is ike a mini application can use the same route with different routes verbs


## What are the ways that a browser can send “data” or request variables to an HTTP server
send it throw the header or the body inside the request object


* **Routing**is the process of selecting a path for traffic in a network or between or across multiple networks.

* **Route prefixes** are associated with routes by design in attribute routing. It is used to set a common prefix for an entire controller

* **Request “Body”** is an properity in the request object that is being sent with HTTP request.

* **Request “Query”**: The req. query property is an object containing the property for each query string parameter in the route

* **Request “Params”** : those are the parameters that are being sent with the url (route)