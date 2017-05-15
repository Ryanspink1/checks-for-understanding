## Week Two - Module 4 Recap


1. What is Webpack and why is it useful?

- It's essentially a bundler for JS. Allows you to pull many different resources together under one, or multiple codebases.

2. When do you want to use event delegation?

- Don't think we did this in class

3. What's one difference between ES5 and ES6?

- functions replaced by hash rockets

4. What's the deal with semi-colons in JavaScript?

- not necessary but helpful for reading. Apparently people are quite opinionated on this.

5. How are you using the MVC design pattern in your Quantified Self project?

- server.js acts like routes, sends to controller --> model --> database --> model --> controller

6. How do you execute raw SQL in node?

using knex: knex.raw(SQL)

7. What is CORS?

-CORS is cross origin resource sharing. It restricts access to resources. 

8. What are some steps to avoid CORS?

const cors = require('cors');

app.use(cors({origin: '*'}));

this opens up resources for any outside entity to access.

#### Review  

9. Why do people say "HTTP is stateless"?

- it doesn't require a server to retain session information.

10. What is a RESTful API?

- an API that follows restful conventions. show, index, create, update, delete

11. What are some main characteristics of a team following an agile workflow?

- breaking things down into small workable pieces

12. What are some advantages/disadvantages to using OAuth to authenticate a user?

- Advantages: putting the burden of security on another entity. If that entity is compromised, your client is too. Your fate is tied with the company you chose to use for oauth.
