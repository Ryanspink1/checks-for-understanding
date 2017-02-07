## Week Two - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!). 

Note: When you're done, submit a PR. 

1. At a high level, what is ActiveRecord? What does it do/allow you to do?

AR is an ORM. It allows the use of object oriented programming with databases. 

2. Assume you have the following model:

```ruby
class Team << ActiveRecord::Base
end
```

What are some methods you can call on `Team`? If these methods aren't defined in the class, how do you have access to them?

all, first, last while, find, sum, average. The methods are inhereted from AR. 

3. Assume that in your database, a team has the following attributes: "id", "name", owner_id". How would you find the name of a team with an id of 4? Assuming your class only included the code from question 2, how could you find the owner of the same team?

Team.find(4).name, Owner.find(Team.find(4).owner_id)

4. Assume that you added a line to your `Team` class as follows:

```ruby
class Team << ActiveRecord::Base
  belongs_to :owner
end
```

Now how would you find the owner of the team with an id of 4?
Team.find(4).owners

3. What do they allow you to do?

It allows me to access the owner table through a foreign key.

7. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.

Many-to-Many relationship

T: Teachers: id, name
T: Students: id, name
T: Teacher_Student: teacher_id, student_id


8. Define foreign key, primary key, and schema.

-Primary key: the unique number/identifier assigned to each object in the database in order of creation(by default)
-Foreign key: In a database relationship between two tables, the foreign key is an attribute of one object where the primary key of it's related object in another table is placed. 
- Schema: is the backbone of the database, defines the structure of the database as it currently exists. 
  
  
9. Describe the relationship between a foreign key on one table and a primary key on another table.

See question 8, 2nd answer.

10. What are the parts of an HTTP response?

Status code, header, body

11. Describe some techniques to make our Sinatra code more DRY. Give an example of when you would use these techniques.

Oof, not sure what is meant by "DRY". I will look it up and make sure I'm on it though. 


### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
2. Name your three favorite ActiveRecord rake tasks and describe what they do.
4. What can you expect from a group as you begin working together? As you continue working together?
5. What two columns does `t.timestamps null: false` create in our database?
6. What cURL flag can you use to send a `POST` request?
7. What case does JSON (and JavaScript) use for multi-word variables?
8. What case does Ruby use for multi-word variables?
9. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
10. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
11. Give an example of when you might want to store information besides ids on a join table.
12. Describe and diagram the relationship between patients and doctors.
13. Describe and diagram the relationship between museums and original_paintings.
14. What are some examples of acceptable values for the parts of an HTTP response?
15. What types of output do we want to test when we test our controllers?
16. What could you see in your code that would make you think you might want to create a partial?
17. Why might you use a helper method?
