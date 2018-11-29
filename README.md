# y2s18-heroku-demo
## Before you start: Fork and clone this repository

1. Fork this repository by clicking "Fork" on this page:
![forking](https://image.ibb.co/jHRieT/forking.png)

2. Copy this repository's url by clicking the green clone button:
![copying url](https://image.ibb.co/n2wYeT/copying_clone.png)

## Part 1: JSON manipulation

## Part 2: Calling your first APIs!
If you visit https://dog.ceo/api/breeds/list/all 
a list of all dog breeds is returned. Try this in your browser! (Chrome/firefox)

Using the `requests` library (as shown in the slides)
Do a GET request to the link above to get all dog breeds and return them
to them as a list to the user as a bullet pointed list

Bonus:
Calling https://dog.ceo/api/breed/<BREED>/images/random

With a <BREED> provided returns an image, example:
 - https://dog.ceo/api/breed/<BREED>/images/random

Create a new route and html page that has a text box, when the user write a name
of a breed it returns an image using the API url above
