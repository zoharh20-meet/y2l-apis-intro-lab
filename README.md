## Before you start: Fork and clone this repository

1. Fork this repository by clicking "Fork" on this page:
![forking](https://image.ibb.co/jHRieT/forking.png)

2. Copy this repository's url by clicking the green clone button:
![copying url](https://image.ibb.co/n2wYeT/copying_clone.png)

## Part 1: JSON manipulation
Start the server by running the app.py file (`python app.py`) and go to the homepage and click around to understand what's already provided for you.

Change the `/movie`function (in app.py). Look at the `json_string` variable change it form JSON string to python dictionary format and return to the user the details about the movie specified in the variable `json_string` 

 - When you visit http://127.0.0.1:5000/movie you should be able to see the title of the movie, the release date, and display an image of the movie
 
### **Bonus:** 
Change the `/tv_shows` function and use the `json_string` variable to show now a list of the tv shows (you will have to change it from a JSON string to python dict like you did before). Visiting http://127.0.0.1:5000/tv_shows should show you a list of TV shows that have name, language, and genres for the show

## Part 2: Calling your first APIs!
The documentation for thefirst API you will be working with can be found here: https://dog.ceo/dog-api/documentation/

If you visit https://dog.ceo/api/breeds/list/all 
a list of all dog breeds is returned. Try this in your browser! (Chrome/firefox)

Using the `requests` library (as shown in the slides)
Do a GET request to the link above to get all dog breeds and return them
to them as a list to the user as a bullet pointed list

### **Bonus:**
Calling https://dog.ceo/api/breed/BREED_NAME_HERE_INSTEAD/images/random

With a <BREED> provided returns an image, Example:
 - https://dog.ceo/api/breed/beagle/images/random

Create a new route and html page that has a text box, when the user write a name
of a breed it returns an image using the API url above
