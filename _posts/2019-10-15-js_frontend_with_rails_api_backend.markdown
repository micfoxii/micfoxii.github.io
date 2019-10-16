---
layout: post
title:      "JS Frontend with Rails API Backend"
date:       2019-10-16 00:30:12 +0000
permalink:  js_frontend_with_rails_api_backend
---


Like all projects, this one put me to the test. The backend was a breeze thanks to all our previous work with Rails, but playing around with DOM from start to finish really started to cement aspects of JS. 

For my project I created an attraction builder for New York where a user inputs Attraction name, address, description, and selects the neighborhood and type (ie restaurant, park, public transit, etc.). Instead of hardcoding the select options, I took the opportunity to populate the options utilizing fetch to retrieve the data from the backend.

![](https://drive.google.com/file/d/1F6yQLv_zrGRWKhZOsfhyNIeXgSYPIKmw/view?usp=sharing)

In the above picture you can see that the corresponding urls are fetched, then the json response is returned, and finally the response is iterated through for each object trigging my render function which will be explained in the photo below.

![](https://drive.google.com/open?id=1nZtUeHc3UF_J5gqfKWGkHo_PmX0eTPrPhttp://)

The render functions selected the appropriate select boxes by using the querySelector to match the object to the id. From this point I created the options to include bothe the name for the innerText of the option and set the value of id to assist in saving the proper object with the attraction.

This allowed for both the name and corresponding id to be set when selecting the object in the form and upon the creation of the new attraction. It also cut down on the time of hardcoding where mistakes could have also been made easily. In the future, it would populate any newly created neighborhoods or types.

There are so many components to JS that have allowed a glimpse of the magic, and I am still learning, but I look forward to continuing to implement and stregthen my skills with the new knowledge I have gained from this section.






