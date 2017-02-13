## Week Three Recap

### Instructions
Fork this repository. Be sure to pull the latest changes to your local repo. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

1. What is the entry at the command line to create a new rails app?

  rails _version_ new name 
  
2. What do Models generally inherit from in rails?

  ActiveRecord::Base
  
3. What do Controllers generally inherit from in a rails project?

  ApplicationController

4. How would I create a route if I wanted to see a specific horse in my routes fitle assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?

  resources :horses, only: [:show]

5. What rake task is useful when looking at routes, and what information does it give you?

  rake routes. It gives you the prefix, verb, URI pattern, and Controller action of each route that is available. 

6. What is an example of a route helper? When would you use them?

  link_to instead of href. Route helpers are used for setting links and paths within your rails app. 

7. What's the difference between what `_url` and `_path` return when combined with a routes prefix?

  url gives the entire URL, thus making it accessible from outside your website. path is used for linking to pages within your site from another page in your site. 

8. What are strong params and why are the necessary?

  Strong params are necessary to limit the information coming from the user that can be set in the db. They're created in the private section of the controller. 
  
9. What role does `form_for` play in helping us create our forms?

  form_for is a form helper. It makes it easier to create and interact with a form than html. 

10. How does `form_for` know where to submit the user's input?

  It has the route from the view it is in(given to it from the controller)? The form label also knows to submit it to the params hash?

11. Create a form using a `form_for` helper to create a new `Horse`. 

  <%= form_for @horse do |f| %>
  
  <%= f.label :name %>
  
  <%= f.text_area :name %>
  
  <%= f.label :breed %>
  
  <%= f.text_area :breed %>
  
  <%= f.submit %>
  
  <% end %>
  

12. Why do we want to validate our models?

  To make sure that we can't create an object without necessary attributes. 
