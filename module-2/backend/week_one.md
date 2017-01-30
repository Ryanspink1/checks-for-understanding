## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb.

 Get: retreive/display info, Post: display new info, Put:save new info, Delete: delete info, Patch: update/fix?

2. What is Sinatra?

 Sinatra is a web app framework.

4. What is MVC?

 MVC is models, views, controllers. It is a pattern put in place to organize information based on functionality.

5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?

 Because it's restful.
 
6. What types of variables are accessible in our view templates without explicitly passing them?

 params
7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
  
  ```ruby
  @count = 1
  get '/horses' do
    erb :index
  end
  ```

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed` to the view?

  ```ruby
  @count = 1
  params[name]="Mr.Ed"
  get '/horses' do
    erb :index
  end
  ```
9. What's the purpose of ERB?

 ERB is a template language that can produce static pages/iterate through Ruby. It helps reduce redundancy of written HTML.

10. Why do I need a development AND test database?

 Develpment and test database must be unique to their environment as information stored in one will differ from the other, due to the separate functions of each environment.

11. What's responsive design?

 Mobile-oriented design that responds to changing the browswer size.

12. What is CRUD and why is it important?

 CRUD is create, read, update, delete. It is a cornerstone of functionality in web development.

13. What does HTTP stand for? 

 Hyper-text transfer protocol.

14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?

 <% Ruby %> and <%= Ruby %>. The first will simply run the ruby code while the latter will display the output.

15. What's an ORM?

 An ORM is an object relational mapper. It writes in object oriented language wrapped around a relational database. Obj classes are mapped to tables in the database.

16. What's the most commonly used ORM in ruby (Sinatra & Rails)?

 ActiveRecord

17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.


18. What's a migration? 

 A migration creates the structure of the database by adding or removing tables.

19. When you create a migration, does it automatically modify your database?

 No. The migration must be migrated, which creates the schema and modifies the database.

20. How does a model relate to a database?

 A model defines an object and it's methods within a table of the database.

21. What's the difference between agile workflow and waterfall method?

 I know what agile workflow is but can't remember waterfall. Waterfall is top down approach to agile workflow or something like that?

22. What is the difference between `#new` and `#create`?

 #new initializes a new object while #create initializes and saves a new object to the database.
