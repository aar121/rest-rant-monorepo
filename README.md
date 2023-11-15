# Project REST-Rant
REST-Rant is an app where users can review restaurants.

## Description and Demo
This application allows users to create new restaurant listings that they like, view restaurants, and leave reviews and comments on the restaurant. Although a demo of this project is currently not available, the full code with a commit history and all dependencies can be found at https://github.com/aar121/rest-rant-monorepo. 

### Technologies 
This application was created using JavaScript, HTML and JSX for the front end and JavaScript and nodeJS for the backend. The database used is Postgres. 

#### Technical Information
Run npm i to install any node packages on your local machine. Then run npm start separately in 2 different terminals, the backend and the frontend. To add to this project, simply fork the project to your GitHub account and add any code on your local machine. Upload your changes to your GitHub account and request to merge with the original directory. 

##### Issues
Although this project is fully functional, in the future we would like to incorporate more styling options that would allow for a different look for the website. We would also like to add the ability to filter based on specific location.


###### API (http://localhost:5000)
| Method | Path                                 | Purpose                                   |
| ------ | ------------------------------------ | ----------------------------------------- |
| GET    | /                                    | Home page                                 |
| GET    | /places                              | Places index page                         |
| POST   | /places                              | Create new place                          |
| GET    | /places/:placeId                     | Details about a particular place          |
| PUT    | /places/:placeId                     | Update a particular place                 |
| DELETE | /places/:placeId                     | Delete a particular place                 |
| POST   | /places/:placeId/comments            | Create a comment about a particular place |
| DELETE | /places/:placeId/comments/:commentId | Delete a comment about a particular place |


###### App (http://localhost:3000)
| Path                  | Component                 | Purpose                                                                         |
| --------------------- | ------------------------- | ------------------------------------------------------------------------------- |
| /                     | `Home.js`                 | Home page                                                                       |
| /sign-up              | `users/SignUpForm.js`     | Form for creating a new user                                                    |
| /places               | `places/PlaceIndex.js`    | List of places                                                                  |
| /places/new           | `places/NewPlaceForm.js`  | Form for creating a new place                                                   |
| /places/:placeId      | `places/PlaceDetails.js`  | Details of a place, including it's comments, and a form to create a new comment |
| /places/:placeId/edit | `places/EditPlaceForm.js` | Form for editing a place                                                        |