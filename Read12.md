[Return to Course 301 Notes](https://KrisDunning.github.io/301-Reading-Notes)

-----

# Reading 12- CRUD

We are using CRUD operations to interact with our Mongo Atlas DB for the Book Shelf project.

## Reading CRUD

In your own words, describe what each group of status code represents:

100’s = Informational codes. Header received and will attempt to serve the request.  
200’s = Success! Request was accepted (not processed per se)
300’s = Redirection codes. Resource isnt here anymore but try again.  
400’s = Client error code. Many different possible issues depending on the code.  
500’s = Server error code. Server could be unreachable or overwhelmed. Possible that its triggered by client.  

What is a status code 202? [CREATE] Accepted. Often used for Asynchronous processing. Processing incomplete but will be in the future.  

What is a status code 308? [READ] Permanent Redirect. Use another URL to access the resource.  

What code would you use if an update didn’t return data to a client? 204. No content.  

What code would you use if a resource used to exist but no longer does? 410 Gone.  

What is the ‘Forbidden’ status code? 403 Forbidden.  

## Video Build a REST API with node, express & mongoDB

Why do we need to pull our MongoDB database string out of our server and put it into our .env?  

- So we dont expose our DB address to the wild.

What is middleware?

- allows/changes the way we interact with our tools/data.

What does app.use(express.json()) do?

- allow us to use any middleware we want. lets server accept JSON as a body.

What does the /:id mean in a route?

- a parameter. we can access with req.params.id

What is the difference between PUT and PATCH?

- update only 1 piece of information instead of all the information.

How do you make a default value in a schema?

- `default: <data>`

What does a 500 error status code mean?

- there is an error on the server.

What is the difference between a status 200 and a status 
201?

- 200 means everything successful. 201 means `create` was successful.  Used for POST routes. 


## Things I want to know more about

async/await/promises. I see they work but I dont understand enough to explain to a 5 year old. Lots of material out there about this luckily.  

-----
