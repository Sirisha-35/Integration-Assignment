# Integration-Assignment
This assignment includes two tasks:

Task-1: Article on Technical Topic
I chose Object Oriented Programming in Python as my technical topic.

Task-2: Create Postman Collection for the APIs
Step-by-Step Process
1. Install Postman and Login to it.
2. Create a new Collection
3. Login API:
   - Send a POST request to the login API.
     POST https://demo.onefin.in/api/v1/usermodule/login/
     
   - In the body, select raw and JSON format. Add JSON and send username and password.
      Sample request:
      {
        'username': 'testuser',
       'password': 'v^4!C%CQ94f0'
      }
 
   - Upon success, the token is retrieved from the response.
     

 4. Movie API: 
   - Use the token from the login API and send a GET request to the movie API in the same collection.
     GET https://demo.onefin.in/api/v1/maya/movies/

   - Add the token to the authorization header: Authorization: Token <token>. The token value is stored in local storage in the login api response.
   - The API will return a paginated list of movies.


