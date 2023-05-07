# Blog
The key concepts in the projetc where:

Basic HTML and CSS (Bootstrap);

CRUD operations with SQLlite and SQL Alchemy - Relational Databases;

FlaskFramework - Basic Functionalities;

FlaskLogin -  Authentication

Python Decorators


## The project
Crete a mobile responsive Blog Website to host posts and comments with Authentication feature. And deploy the app on Heroku. As there is a chance that the blog will not be hosted for a long time, the basic app features are presented below.

## Home Page
![image](https://user-images.githubusercontent.com/124715795/236660267-80a4c79d-b78f-4eae-8976-9f2c0ded2156.png)
The Home Page display a NaviBar with : Home, Login, Register, About, Contact
Create New Post redirects you to the Forms to create a new post. The acess is retritcted to Admin Only. To that the login is necessary.

## Login Page
![image](https://user-images.githubusercontent.com/124715795/236660501-8bb8fab5-7ab1-41fa-a1be-890e2f093f4e.png)
We have two entries of a Flask-WTForm - one for the email and the other for the password. When submitted, it will be checked against the user database. If it is a register user will have the permission to comment, if admin can create a new post too.

## Create a New Post
In this section is displayed the form to create a new blog post. With a title, subtitle, img_url and body sections to fill. The data from the for is stored with SQLAlchemy after the POST request (submit button).
![image](https://user-images.githubusercontent.com/124715795/236661457-af44a703-cff9-45e6-87b1-c4856bd20914.png)

## Home Page displaying the new posts

![image](https://user-images.githubusercontent.com/124715795/236661844-7d4bceea-6490-45e3-b430-28c3eaa0670c.png)
Now, when we redirect to the home page we can see the new blog post presented with it's title, subtitle and the user who post it.

## Show specific blog post
![image](https://user-images.githubusercontent.com/124715795/236662545-85c90d50-96c5-45b4-b04b-891d6e4507d6.png)
![image](https://user-images.githubusercontent.com/124715795/236662570-39b78373-3483-4769-9d83-d55bbe6e45b1.png)
Here we see the complete post, the edit button and the comment form. If we submit a comment:

![image](https://user-images.githubusercontent.com/124715795/236662654-2127e708-c228-4d2f-8ed1-8479cf02fc6f.png)

## Post edit
When the 'edit post' page is loaded, the forms are automatically filled with the post information to be edited.
![image](https://user-images.githubusercontent.com/124715795/236663985-fb166d3e-18d8-440e-8906-553b15e68405.png)

### Authentication 
If user that is not the admin and tries to edit or create a post:
![image](https://user-images.githubusercontent.com/124715795/236662839-bf4238a4-5c35-4733-9313-849ab3e2a022.png)

### Adding more posts
![image](https://user-images.githubusercontent.com/124715795/236663264-a5ba09b3-10d9-4b7b-8606-9ca73b9058c5.png)
![image](https://user-images.githubusercontent.com/124715795/236663308-ec722ff9-54fc-44a3-8e9e-c4b57ef7d93d.png)

### Using DBBrowser to see the tables in the Database
![image](https://user-images.githubusercontent.com/124715795/236663557-ba999442-c184-42e7-a6ee-e42dcd146280.png)
![image](https://user-images.githubusercontent.com/124715795/236663573-eeda8727-cf18-4043-8b67-284e28437dfd.png)
![image](https://user-images.githubusercontent.com/124715795/236663604-33ae6b7c-decf-4074-82c1-9869482bb730.png)

We can see that the relationship between the tables and the hashing of the password is working properly.
There are a few comments in the code highlighting some key structures and resources used.


