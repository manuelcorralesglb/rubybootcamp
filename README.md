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
#### Reading material
#### Excercises
Create a model, create a controller, create a route, create a view.
#### Key points
#### Extra credit


### Topic 4: Tests first
#### Reading material
#### Excercises
Create a test for a new feature, see it fail, implement the feature.
Cucumber, capybara and rspec.
#### Key points
#### Extra credit

### Topic 5: Adding a second model
#### Reading material
#### Excercises
#### Key points
#### Extra credit

### Topic 6: REST and JSON
#### Reading material
#### Excercises
Make the app serve JSON for the features already implemented.
Jbuilder
#### Key points
#### Extra credit

### Topic 7: Adding a third model
#### Reading material
#### Excercises
Ideally using a different relation cardinality than the fist one
#### Key points
#### Extra credit

### Topic 8: Asset pipeline
#### Reading material
#### Excercises
Add foundation, bootstrap or semantic-ui to the app. Make also your own styles. Run the app in production mode.
#### Key points
#### Extra credit

### Topic 9: Adding a second model
#### Reading material
#### Excercises
#### Key points
#### Extra credit
