---
layout: page
title: Manoa Student Kitchen
---
<img class="ui image" src="../../images/MSK_Home.png">

Manoa Student Kitchen is an web-based application designed using Meteor, Semantic UI and Underscore that provides the ability for students at UH Manoa to share recipes that are tailored to the UH Manoa campus and culture. The app was my final project for ICS 314 (Software Engineering), and I worked in a team of three with other students at UH Manoa.

[For more information about the project, you can view the project page here.](https://manoastudentkitchen.github.io/)

## Structure

Manoa Student Kitchen was built using the Meteor framework, utilizing:
* [BlazeJS](http://docs.meteor.com/api/blaze.html) to create dynamic templates for the user interface
* The [publication and subscription API](http://docs.meteor.com/api/blaze.html) to handle the MongoDB Collection database
* [FlowRouter](https://guide.meteor.com/routing.html#flow-router) to perform client-side routing of the URLs

The app also utilized [Semantic UI](https://semantic-ui.com/) for interface assets and [Underscore.js](http://underscorejs.org/) for JSON manipulation.

## Features

In the app, users could add and edit their own recipes, search for recipes made by others, and view and tag others' recipes.

The tagging system was based on [Steam tags](http://store.steampowered.com/tag/), allowing for users to define their own tags to apply to each recipe. For example, a user might tag a recipe to be "spicy", "quick" or "pescatarian-friendly", and others can vote on those tags if they agree or not. This allows us to forego a traditional category system and provide a more user-oriented and dynamic environment.

## Contributions
<img class="ui image" src="../../images/MSK_View_Recipe.png">

My contribution towards the project consisted largely of designing the interface front-end and the database backend, as well as some integration in between. I implemented the relational model for database management for the app, with recipe documents, users, tags, ingredients and locations each having their own Mongo.Collection, and leveraging the built in id field as keys. We had tags, ingredients, and locations to be separate from recipes, because I wanted to allow for simpler querying of recipes with a certain tag name, or a specific ingredient, or locations to provide information about what recipes could be available from just ingredients from that store. Ultimately, only the tag-based queries were implemented, and the other features are available for further development of the app.

Much of my time leading up the later milestones was spent on the "View Recipe" page, which pulls data from the Collections based on the ID of each recipe. To do this I set the FlowRouter to contain the recipe's ID as a parameter, and used it in combination with Underscore.js to generate a queries in Meteor template helper functions to provide the recipe object and the corresponding tag, ingredient, and location objects. For the list of ingredients, I used a BlazeJS template along with the helper functions.

In the tag input, I implemented a feature that suggests tags from other recipes by using a [Local Search](https://semantic-ui.com/modules/search.html#local-search) from Semantic UI, in combination with a helper function.

## Takeaways

It goes without saying that this project was an invaluable exercise for me in various languages and frameworks, as well as design for both front-end and back-end development. After the past few months I've become far more comfortable in HTML, CSS and Javascript and now I have practice with tools like Meteor that I can utilize for new projects. Furthermore, it was my largest scale coding project in collaboration with other students, and the first to utilize project management techniques like milestones and various Github tools.
