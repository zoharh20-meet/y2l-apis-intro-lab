## Before you start: Fork and clone this repository

<!-- 1. Fork this repository by clicking "Fork" on this page:
![forking](https://image.ibb.co/jHRieT/forking.png)-->

<!--2. Copy this repository's url by clicking the green clone button:
![copying url](https://image.ibb.co/n2wYeT/copying_clone.png)-->

## Part 1: JSON manipulation
A. First we'll start the server. Do this by opening terminal, cd-ing into the folder you clones, and running the app.py file (`python app.py`).

B. In a web browser, go to the homepage and click around to understand what's already provided for you.

C. Look at the `movies()` function in `app.py`. In order to use the information from the JSON string, we need to turn it into a python dictionary. Take a look at slide 22 to see how to use json.loads. 

D. Now we need to pass the dictionary into `render_template`. On line 23 of `app.py`, your code should look something like: `return render_template('movie.html', movie=PYTHON_DICTIONARY_HERE)`.

E. When you visit http://127.0.0.1:5000/movie you should be able to see the title of the movie and an image of the movie. But notice that the release date is not shown! Look at `movie.html` and fix it to show the movie's release date.
 
### **Bonus:** 
Change the `/tv_shows` function and use the `json_string` variable to show now a list of the tv shows (you will have to change it from a JSON string to python dict like you did before). Visiting http://127.0.0.1:5000/tv_shows should show you a list of TV shows that have name, language, and genres for the show

## Part 2: Calling your first APIs!
The documentation for thefirst API you will be working with can be found here: https://dog.ceo/dog-api/documentation/

If you visit https://dog.ceo/api/breeds/list/all 
a list of all dog breeds is returned. Try this in your browser! (Chrome/firefox)

Using the `requests` library (as shown in slide 25)
Do a GET request to the link above to get all dog breeds and return them
to them as a list to the user as a bullet pointed list

### **Bonus:**
Calling https://dog.ceo/api/breed/BREED_NAME_HERE_INSTEAD/images/random

With a <BREED> provided returns an image, Example:
 - https://dog.ceo/api/breed/beagle/images/random

Create a new route and html page that has a text box, when the user write a name
of a breed it returns an image using the API url above
