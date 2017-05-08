## Week One - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's the most useful thing you learned from completing the intermission week work?

  - The sorting problems helped bridge the gap between ruby and JS

2. What are some tools to help debug JavaScript code?

 - debugger, eval(pry.it), console.log()
 
3. What are some tools you need in order to unit test your JavaScript?

 - Chai, Mocha

4. What is the syntax for invoking a function?

  function(); 

5. What's the difference between `==` and `===` in JavaScript?

 - === and == are the same except with === the types must be the same

6. What's the difference between asynchronous and synchronous JavaScript? 

  synchronous means flowing in order, async doesn't wait for functions to complete before moving on to the next

7. What's a callback function and what are some reasons when we use/need callback functions?

- callback functions are functions that are passed to other functions as a paramter. Helps w/async?

8. What's the biggest difference between a promise and a callback?

 - callbacks and promises are mostly the same, except promises work in order

9. How do we setup a route when creating an API with Node and Express?

  - app.get('/api/secrets/:id', (request, response) => {
  const { id } = request.params;
  const message = app.locals.secrets[id]

  if (!message) { return response.sendStatus(404); }

  response.json({ id, message });
});

10. What's `npm` and what do we use it for?

- NPM is node package manager. Can be used to install node packages. Can also be used to run commands in express. 

#### Review  
11. What's the MVC design pattern? Describe each part of MVC?

- MVC is model, view, controller. Controller receives the request/route, sends qury to the model which accesses info from the database and then sends it back to controller when renders the view for the user.

12. What is AJAX? What are some benefits of using AJAX?

 - AJAX is a api request system in JS that creates the request without reloading the page. One benefit of this is that the user is not left hanging waiting for a response from the api for the page to load and will have something to look at other than a loading screen.

13. What's a background worker? When would we want to use a background worker?

- a background worker allows you to run a separate thread. It's useful when you don't want the page to wait for things to happen (ie sending automatic emails) before it loads.

