First Express
======

This is a single resource API using Express. We will use a light-weight in-memory model instead of using a database today.

## Directions

This is a **solo** lab.

* Pick a "resource" for your API, like `unicorns`
* Implement:
    * `GET /<resource>` - returns array of all of the resources
    * `POST /<resource>` - inserts the supplied request body as a document into the resource collection
    * `GET /<resource>/:id` -
      * returns the single object specified by the id
      * returns 404 not found if no resource found with that id    
    * `DELETE /<resource>/:id` - removes the resource with that id
      * **not** an error if doesn't exist. 
    * `PUT /<resource>/:id` - updates the resource with supplied request body
* Use plural name in your url path (`/unicorns`, **not** `/unicorn`)

## Architecture and Design

* Use the **structure** we used in class.
* Follow the **process** we used in class to build up both your model and route

## Testing

* Create a dedicated `request.js` helper class for opening the http server

## Rubric

* Server, App, Project Organization: *1pt*
* Each tested API endpoint
  * `GET` all: *1.5pts*
  * `POST`: *1.5pts*
  * `GET` by id: *1.5pts*
  * `GET` by id with 404: *1.5pts*
  * `PUT` by id: *1.5pts*
  * `DELETE` by id: *1.5pts*
