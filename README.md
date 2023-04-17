# CS-465_Project
Course project for CS-465
## Architecture

  ### Compare and contrast the types of frontend development you used in your full stack project, including Express HTML, JavaScript, and the single-page application (SPA).
  
  The two types of front end development we did for this project was server-side rendered HTML templates with handlebars and client-side rendered pages as a SPA with Angular.  With the server-side rendered version, everything is rendered on the server, before it's sent out to the client.  Although this performs better for search engine optimization, it puts more strain on the server and decreases CPU usage for the server to respond to incoming requests.
  
### Why did the backend use a NoSQL MongoDB database?
  The backend used a NoSQL MongoDB database to store the trip data.  The data in a NoSQL db is more intuitive to work with when programming apps with JS.

## Functionality
  ### How is JSON different from Javascript and how does JSON tie together the frontend and backend development pieces?
  JSON is merely a way to structure data that is in similar syntax to a JS object, while JavaScript is a programming language heavily used for web development.  The data injected into the app in this project was sent as BSON to JSON from the MongoDB to the front end client to render the trip data for the SPA.
  
  ### Provide instances in the full stack process when you refactored code to improve functionality and efficiencies, and name the benefits that come from reusable user interface (UI) components.
  We refactored the code to be a SPA, after the user was logged into the site.  Based on JavaScript condintional statements the user was presented with a different page layout/template.  Since all of the components for each "page" were already on the client, this made redirects to content much more efficient.
  
## Testing
  ### Methods for request and retrieval necessitate various types of API testing of endpoints, in addition to the difficulties of testing with added layers of security. Explain your understanding of methods, endpoints, and security in a full stack application.
  In order to add or edit a trip, the user had to be logged in.  Once the user was authenticated, the user was authorized to add and edit trips.  If the user was not authenticated, they did not have sufficient authorization to add or edit trips, so the trips were read-only to the unauthenticated user.
  
## Reflection
  ### How has this course helped you in reaching your professional goals? What skills have you learned, developed, or mastered in this course to help you become a more marketable candidate in your career field?
  Any web experience is good experience.  This course helped me develop the fundamentals needed to expand upon to join a development team or to create my own applications.  Since most data can be sent to an interface with API endpoints with or without authentication, depending on the type of data sent, the possibilities are plentiful.  Even if just using this for oneself, with all of the smart devices nowadays, someone could use these skills to develop their own app for monitoring their home security devices, network, and other smart devices while away from home, although some of those connections would require web sockets.  Or commercially, someone could develop an app that monitors personal/business finance, investments, weather, or any other useful data capable of being sent from one location to the user's location.
