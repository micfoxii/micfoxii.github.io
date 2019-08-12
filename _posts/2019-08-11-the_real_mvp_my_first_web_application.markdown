---
layout: post
title:      "The real MVP, my first web application."
date:       2019-08-12 00:03:44 +0000
permalink:  the_real_mvp_my_first_web_application
---


I have come a long way since the first portfolio project. What I thought was a failure was not so bad, and I worked through the first portfolio with a level head. Ultimately, from my assessment, I realized I knew more than I let myself believe from discussing my code in my review. From that takeaway, I began my Sinatra web application with the understanding that I approached everything one step at a time.

For my project I decided to create a website called iTravel that kept track of users' travel reviews, since travel has always been something important to me. In this web application a user is able to create and login to their account, create, read, update/edit their destinations, and delete their destination entries. Besides having access to their travel reviews, the users also have access to read other user reviews of their travels.

To first begin building iTravel, Sinatra was installed and required in my gemfile and set within the environment file. In the application controller, the class ApplicationController inherited (<) from Sinatra::Base. Two additional controllers were created (destinations_controller and users_controller) where each class inherited (<) from ApplicationController class allowing Sinatra to be utilized within these controllers. Through using this web framework, I was able to create a simple dynamic website.

Another important piece to this website was the utilization of ActiveRecord. This ORM (Object Relational Mapping) allowed interactions between my Models, Views, and Controllers (MVC) with the databases I created. Through migrating my tables of Users and Destinations, the MVC and tables could pass information back and forth dependent on user inputs.

This passing of information allowed for the user to view the processes of Creating, Reading, Updating (editing), and Destroying/Deleting of data. This was accomplished through routes establish in the controllers, utilizing RESTful Routing. This pattern of RESTful Routing was an important concept to understand because it is a pattern consistent across well designed web applications.

The RESTful Routing patterns consist of HTTP verbs GET, POST, PUT, and DELETE and CRUD actions CREATE, READ, UPDATE, and DELETE. These patterns are important since devs often work alongside other devs, and if you create routes that work but only you understand - what good is that? This could be an entirely different post, so if you would like to read more about this importance follow this [link](https://medium.com/@thejasonfile/restful-routing-2056f799223e) to an article written by Jason Arnold, a Flatiron graduate.

Other important aspects of this project were my has_many and belongs_to relationships between users and destinations. Users have_many Destinations and Destinations belong_to Users. The along with those relationship, the foreign key user_id located in the Destinations table allowed for CRUD to function and the views utilize code to build the dynamic web application.

The list could go on and on regarding various aspects of the project including validations to ensure unique user email/username and required form information, bcrypt to secure passwords, protecting data through redirects and authorization, helper methods, and error messages. I will address some of these in future posts to allow for more detail in specifics.

Through trial and error, googling, and continual testing the curriculum really solidifies by the time I finished the project. While it was not easy, my first Sinatra Web App stretched my mind in terms of understanding core concepts, and it also thinking of possibilities to take things further. I am excited to continue learning, thinking of possibilities for application to simplify the human experience, and ultimately developing more complex things. 
