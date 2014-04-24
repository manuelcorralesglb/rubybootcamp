Ruby bootcamp
============

Globant's Ruby Boot Camp is a hands on training course covering the following topics: ruby language, rails framework, basic HTML, CSS and javascript; and REST/JSON APIs with ruby.


![image alt text](https://www.ruby-lang.org/images/header-ruby-logo.png)



Material:

http://www.codecademy.com/tracks/ruby

https://www.bloc.io/ruby-warrior/

apigee REST APIs desing book


###Technical Assistance

You can contact other bootcamp participants or any available tutor if you need technical assistance. We will create one chat for boot camp members only, and another one for boot camp members and tutors when boot camp starts.

###Performance Measurement

1. Code review after each practice and sprint

2. Checkpoint completion after Learning stage with your assigned tutor



###Materials

1. The IDE to use is [SublimeText](http://www.sublimetext.com/). (You are free to use other IDE)

2. Installed ruby using rvm

3. Skype Account + headset (audio calls)

4. Create your own[ GitHub](https://github.com/) account. Follow this[ guideline](https://help.github.com/articles/set-up-git) to setup your account. 

5. Create a new repository in[ GitHub](https://github.com/)  to host the project code.

6. REST client (POSTMAN recommended)



###General Guidelines

The boot camp is organized in the following way:

##Learning days

###Topic 1: Ruby basics
  1. Create a game in which the user has to guess a number.
  2. The number to be guessed must be initialized randomly in the constructor.
  3. The constructor must take as a parameter the max attempts the user have to guess the number.
  4. The game must indicate the user if the number entered is bigger or smaller than the one he has to guess.
  5. The game should keep track of all the numbers the user entered.
  6. When the user wins, a message should be displayed to the user telling so and also a score should be printed. The score should be calculated based on the attempts the user did and the max amount of attempts it had.
  7. The user lose if exceeds the limit of attempts.
  8. Add a method that prints all numbers the user entered.


### Topic 2: Inheritance, polymorphism and duck typing
  1. Implement a hierarchy of Person, Student and Teacher.
  2. Implement a method “introduce_me” in each of the classes that prints something like: “Hello, my name is Juan and I am a Student”.
  3. Create an array that contains at least one instance of each of the defined classes, loop through it and invoke the introduce_me method.
  4. Remove the inheritance relationships and repeat the step 4. (Duck typing)
  5. Implement a module with the following methods (hint: all methods should rely on an “age” method not implemented in the module):
    * can_drive?
    * can_vote?
    * can_travel_alone?
  6. Implement an “age” method in Person, Student and Teacher and the include the module in the classes to create a mixin. Call the methods implemented in the module in instances of the classes.

### Topic 3: Rails MVC
  1. Create a new rails application named rails_bootcamp.
  2. Generate a model and migration called Team using the "rails generate" script. Team must have this fields: name, logo_image and stadium_image.
  3. Run the migrations using rake.
  4. Open the rails console (rails console) and create a few teams. Then query the teams using ActiveRecord methods:
    * Team.where(condition)
    * Team.all
    * Team.first
  5. Generate a controller TeamController. Implement a method named show that fetches a Team by id and assign it to an instance variable @team.
  6. Generate a view that displays the Team name and show the team image (you have to use the instance variable declared in the controller to access the team)
  7. Create a route in the routes.rb that hits the method show in the team controller.
  8. Try the app by hitting the url defined in the routes file using a browser.

Key points:
  * The page should display the team name and logo and the stadium picture.

Extra credits:
  * Add stadium coordinates to the model and display the location of the stadium in a google map embedded in the page.

### Topic 4: CRUD
  1. Create a new route, a new method in the controller and a view to display a form to create a new Team.
  2. Implement all steps needed to have a page that lists all the teams.
  3. Add edit and delete links next to each team in the listing page.
  4. Implement the edit and delete actions.
  5. Add validations to the Team model so the name can't be empty when creating or updating a Team.

Key points:
  * Use Rails convention to name the methods in the controller.
  * Use Rails form helpers.
  * Use Rails link helpers.
  * Reuse the form in both create and update pages by creating a partial.

### Topic 5: REST/JSON
  1. Add the jbuilder gem to the Gemfile (if not already present)
  2. Create a jbuilder template to get a JSON response for a Team.
  3. Complete the CRUD operations using JSON.
  4. Try it using the POSTMAN REST client.

Key points:
  * Use the respond_to method to render the json response.
  * Use the correct http status codes in each case.
  
### Topic 6: Relations (part 1)
  1. Create a new Match model that should have at least a time field and two teams.
  2. Link the Game and Team models using the ActiveRecord relations.
  3. Create a new page to create Matches.
 
### Topic 6.1: Relations (part 2)
  1. Create a Group model and link the Match to a Group using ActiveRecord relations.
  2. Create a page to create Groups.
  3. Create a page to add matches to a group.
  4. Create a page that lists the groups.
  5. In the page created in point 7, make the group name a link that takes you to the group matches. Matches should be sorted by date.

Key points:
  * You should have a has_one and a has_many relationship.
  * You should have validations in the Group and Match models.

Extra credit:
  * Create a new model Stadium and refactor the Team model to move out the stadium properties to his own class. Make a relation between Stadium and Team.
  * Add a relation between match and stadium (where the match will be played).

### Topic 7: Testing
  1. Include rspec, factory girl and Capybara gems in the Gemfile.
  2. Write factories for teams and matches.
  3. Write a capybara test that verifies the creation of a Team.
  4. Write a capybara test that verifies the creation of a Match.


### Topic 8: Beautify the app
  1. Include bootstrap css and js into the project (use the vendor folder).
