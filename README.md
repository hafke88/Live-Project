# Live-Project
The final project implemented during my Python Developer Bootcamp



## Introduction
During the last two weeks of my time in the Python Developer Bootcamp, I worked with fellow developers developing our own personal app using the Django Framework. This was a tremendous opportunity to see how teams work utilizing Agile/Scrum aiming towards the same goal of completing the project. There were many parts of the project that were fresh in my mind on how to complete and without fail, there were several parts of the project that presented a great challenge, which took patience and constant grit to get right. Fortunately, in the end, I was very satisfied with the app I built relating to one my passions, exercise. I have many more ideas to expand on this app and I will hope to continue on this again one when I become a more seasoned developer.

Below, you can follow me though my journey of tasks assigned during the live project. As the stories progessed so did the challenges that came with them. 

### Story 1 Build Basic App
The assignment here was to create a new app, register the app, create base and home templates using the correct block tags, add function to the views page to render the home page, register urls with the Mainapp, link my personal app's homepage to the project's homepage by adding an image link and finally, adding some miniaml content like a navbar, background, title and footer. 

In my opinion, this was one of the easier assignments, but also demanded a fair amount of time. A lot of commands executed were executed in the terminal to get started. I knew what I wanted in my project and to build off of that, I drew up what I wanted to include in my navbar. I felt this approach would give me a direction to head in. After advancing further in the project and knowing my limits, I took out the about link from the navbar. 

![image](https://user-images.githubusercontent.com/85956976/134739231-a96c9fe5-0436-4837-a39d-ea0a0bb089b3.png)

### Story 2: Create your model
Story 2, was to create a model for the collection item you will be tracking and add the ability to create a new item. Creating a form that would receive user input was easy to know when building this exercise app. 

To explain further, below is my form and models file with all the fields I wanted to have given to the user. Conventional workouts, in my opinion, are the cream of the crop when it comes to exercise. Any person can take several exercises for one target muscle group and apply them in their daily routine. 


#### The form grabbed all the fields from my models file
![image](https://user-images.githubusercontent.com/85956976/134738874-d03237c8-bbb9-443d-b59b-750e0fc18f64.png)
      

#### These were the fields, along with the choices for choosing exercises in a specific muscle group
![image](https://user-images.githubusercontent.com/85956976/134738795-d5dd5eeb-e318-4b38-87ce-c678d0d9e790.png)
        
### Story 3: Display all items from databas
This assignment was to display information from the database in a page. This was another fairly straightforward assignment in terms of rendering the information from the database. Using the correct tags to call in 'name in names' from the views file, the html page displayed all exercises from the database with their respective items.

#### Create a new HTML page, link it from your home page
Due to the background image, I had to change the style slightly so the font was legible.
![image](https://user-images.githubusercontent.com/85956976/134739926-7c330abc-062e-4867-97cf-a71c8566a852.png)

#### Add in a function that gets all the items from the database and sends them to the template
Names called all objects from my Excerises class off of the model file.
![image](https://user-images.githubusercontent.com/85956976/134739879-bcf7e2c6-95cf-40d1-b72b-03acc2aac2e8.png)

### Story 4: Details Page
For this story, we had to create a details page that will show the details of any single item from within the database, as selected by the user. Link this to the index page for each item. This actually posed the biggest challenge to me. I had written out code, which I'll share below, that did not render the details the way I expected it to. I had to reach out to an instructor for help and after a while, it came down to simplifying my code. I wasn't too particularly happy about this but it did complete the assignement and earn me a pass. 

From the names file:
![image](https://user-images.githubusercontent.com/85956976/134741949-f8a819f4-8e92-44a6-bbd9-8d57ba0cefd9.png)

From the details file:
![image](https://user-images.githubusercontent.com/85956976/134742210-a1e51d29-a8e9-4952-8d12-336e0a6d99bd.png)

However, all weekend, it bothered me to know that my webpage didn't render the styling or the details in container like I wanted it to. I was given all the exercises as links and when you clicked on each link, it brought up a not so good looking render of my exercise details. That following Monday, instead of moving forward with Story 5, I went back into my code to try once more. Again, I was stuck. I think I tried for close to five hours before I reached out to another instructor who could help me go at this problem again. 
Long story short, it came down to proper syntax and calling the right url. Changing that line of code  for my options tag from my original template to 
"{{ name.pk }}/exercises_details/" executed exactly what I needed to have done.


### Story 5: Edit and Delete Functions
In my final story for my live project I had to allow for edits and delete functions to be done from the details page or from separate pages. Also, I had to have confirmation before deleting. This was done by adding a form to allow an edit in my function on the views page. The 'ExercisesForm' will render the exercise and its details to the user and allow the user to add, edit or delete any information to the exercise stored in the database.

![image](https://user-images.githubusercontent.com/85956976/134743194-d6491d23-88d8-4ab0-a3bd-7b12f77388fb.png)

My delete buttons were formed by creating a path to a final 'are you sure' before actually deleting any exercise from the database.

![image](https://user-images.githubusercontent.com/85956976/134743389-50573b75-1f8c-4725-a210-6a28c3b6c577.png)
![image](https://user-images.githubusercontent.com/85956976/134743441-555e5fe0-d36e-4fb7-9fcd-66aeddcffd53.png)


