## Week Four Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

* What is a cookie?

  -a cookie is data stored on a local computer to store stateful information like passwords, login status, etc. 
  
* What’s the difference between a session and a cookie?

 - a session is temporary and only lives within the time one is browsing a particular website, or less. It can be used with cart items, and login status. 

* What’s a flash and when do you want to use flashes?

 - flash messages are a system for showing particular messages regarding success, failure, alert, and notice. They can be customized for alternative topics as well. They can be stylized and read a message across the screen. 

* Why do people say “HTTP is stateless”?

 - HTTP is stateless because of how it deals with every single transaction independantly. The request and response are not linked as one transaction.

* What’s authentication? Explain.

 - Authentication is the process of verifying that the password you've entered is you and logging you on as a user. A password is checked using bcrypt and if it matches up, a session is stored as a user. 


* What’s the difference between authentication and authorization?

 - authorization is the program checking to see if your account has permissions to a certain part of the software, be it a database or a web page. If you have the permissions, you are granted access to the restricted content. 


* What’s a before filter?

 - a before filter is a class method in rails. It allows one to refactor the controller by running certain lines of code automatically to specific routes so that the line of code is not redundantly called. It is set within the private section of the controller. 

* How do we keep track of a user once they’ve logged in?

 - user sessions are stored in a sessions hash to keep track of a logged in user. Also, cookies can be used to keep track of the user. 


* When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?

 - namespacing is used when limiting access to certain routes, as one would in the case of restricted admin views. Resources are nested when you want to show direct ownership of related objects. Namespace is authorization, nested resources are ownership. 

* At a high level, what tools can you use to implement authorization? How would you use them?

 - using roles is one way to implement authorization. A binary role (0) is given to a regular user as a role attribute while an admin is given (1). Admin access is given to users with the role 1, while a regular user experience is provided for a user with the role 0.


* What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?

 - enum is used to give a static, changeable attribute to an object. It's great for working with a particular status of an object that will need to be changed. An enum needs to be in your database? Or an integer to denote 1 or 0 as a status? The enum is declared in the model of the object you're working with.

* What are some strategies you can use to keep your views DRY?

 - creating a universal form for the new and edit routes is a great way to keep views DRY. Not sure what other good stategies there are other than iterating correctly and moving logic as close as you can get to the model. 
