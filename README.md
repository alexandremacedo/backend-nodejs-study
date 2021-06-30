# backend-nodejs-study

NodeJS, allow us to run javascript application on server-side

v8 -> Google creation to translate node to browser
libuv -> Built to node work better with async way
modules -> Multiple modules to use in code

Evevnt loop -> Listen reqs and send to call stack
  * Call stack -> Stack functions 

Single thread

Non bocking I/O -> Execution more than 1 function 

Packages
  * Npm and Yarn
  * Install packages and fornecer packages


REST and RESTFull

API (Application Programming Interface) -> Rules and especifications that allow us to interact with the application
  API documentation is the api heart
  
REST () -> Is an architetural model, if we use their concepts we hits the RESTFull API
  6 Rules for REST
  * Client - Server -> Se preocupa only with his implementations
  * Stateless -> Server doens't store states
  * Cache
  * Interface
    * Resources
      ID -> Their routes: api.com.br/users
      Representation -> Provides the data with differents formats like JSON, XML.
      Messages -> Return clean messages to tell about errors, success.
      HATEOAS -> Return links
  * Layers -> Allow to set load balancing between the application
  * Needed Code -> Had to implements another functions to client
 
HTTP Verbs

GET -> Return data
POST -> To store data
PUT -> To update data
DELETE -> To delete data
PATCH -> To make partial updates

HTTP Codes

1xx -> To inform
2xx -> To confirm
  200 -> Success requisiton
  201 -> Created -Success insertion
3xx -> To redirect
4xx -> Client error
  400 -> Bad request
  401 -> Unauthorized
  403 -> Forbidden
  404 -> Not found
  422 -> Unprocessable Entity
5xx -> Server error
  500 -> Internal server error
  502 -> Bad gateway
  
  
Requisiton Params
Header -> To send token, method in reqs.
Query  -> Starts in the and of url, before "?"
  api.com.br/users?page=1&type=admin
  Key -> Id of param
    In this case: page and type
  Value -> The content of a key
    In this case: 1 and admin
  Separator -> Indicate that param ends
    In all cases: &
Route -> Inside de url
  api.com.br/users/{id}/history
  In this case: id that could receive a value
  api.com.br/users/10/history
Body -> Send in the body
  In this case: JSON{
    "name": "Alexandre"
  }
