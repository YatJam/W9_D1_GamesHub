# W9_D1_GamesHub

Homework: Full Stack Games Hub App

Task
Draw a diagram showing the dataflow through the application starting with a form submission, ending with the re-rendering of the page. This will involve a multi-direction data-flow with the client posting data to the server and the server sending data back to the client with the response. Detail the client, server and database in the diagram and include the names of the files involved in the process.

![Getting Started](/W9_D1_GamesHub/data_flow.png)


Questions:

1) What is responsible for defining the routes of the games resource?

1a) create_router.js utilising express.

2) What do you notice about the folder structure? Whats the client responsible for? Whats the server responsible for?

2a) The client is responsible for the front end elements of the app, the localhost:3000 where the react app operates. The server is the back end, containing the database (in this case) and handles the requestes to the database from the front end.

3) What are the the responsibilities of server.js?

3a) connects to the database and has access to the different restful route methods whenever any CRUD is requested by the front end.

4) What are the responsibilities of the gamesRouter?

4a) To define the specific functions of each CRUD element when a request/response is made.

5) What process does the the client (front-end) use to communicate with the server?

5a) RESTful routes

6) What optional second argument does the fetch method take? And what is it used for in this application? Hint: See Using Fetch on the MDN docs

6a) response, returns a promise that resolves with the result of parsing the request body as JSON

7) Which of the games API routes does the front-end application consume (i.e. make requests to)?

7a) PUT

8) What are we using the MongoDB Driver for?

8a) it allows Node.js applications to connect to MongoDB and work with the data.

Extension

E1) Why do we need to use ObjectId from the MongoDB driver?

E1a) This is because MongoDB uses object ids (_id) as its method for identifying specific elements in a respective collection.

Add to your diagram the dataflow for removing a game.

![Getting Started](/W9_D1_GamesHub/data_flow_extension.png)

