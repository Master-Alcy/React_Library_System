# Library_System

The bundle.js is uploaded now, for people to use just npm install and npm start to test the website. The server router will start with the client router for easier testing (Location: server/routes/index.js), but they can be seperated easily.  

## My Contribution

I was building the whole front-end react and back-end router. This is the first time I'm using react and I found its components can seperate functionality of the website easily, which makes the development of each part of the website clearer. I tried not to write react inside the html directly which may reduce the readability.

## Some Idea

Origin repository at <https://github.com/Master-Alcy/StevensCodes/tree/master/CS-546-2018F/FinalProject>  
Team repository at <https://github.com/CS546-Team/Library_System> where you can see the contribution to the project.

Since it's hard to group all of teamates together everyday, the usage of github and VSCode Live Share are important. Testing website is extremely important to find bugs and place to be improved. Thus we use documents/Feedback.md for people to give their feedbacks and ChangeLog.md to say if things are fixed or unhandled and why

## Installation

For installing bcrypt, following instructions on this page:  
<https://github.com/kelektiv/node.bcrypt.js/wiki/Installation-Instructions#microsoft-windows>

Install Environment:  
npm install

Start server/index.js (our main):  
npm start  

(Optional) Seed Databse (Note that you can use website to seed database yourslef):  
npm run seed  

**Important Note**:  
The mocked username/real_password and bookTitle/ISBN are printed in console for testing only. Else all passwords are stored as hashed and can't be tested in login.

## For Development

Use nodemon:  
npm run server-dev  

Use webpack and install bundle.js:  
npm run react-dev  

(optional) Use --optimize-minimize and --define process.env.NODE_ENV="'production'":  
npm run build  

For development, it's easier to use both nodemon and webpack.

## Structure

Intro:

A simple website for managing library about rental, storage and possibly selling operations for students and staffs.

Core:

1. User function:
   1. sign in:
      1. two types: student, staff
      2. user name
      3. check valid password(AJAX)
   2. log in:
      1. user name
      2. password (AJAX)
2. Studnet function:
   1. search books
   2. check records
3. Staff function:
   1. add new books
   2. remove old books
   3. rent books to students
   4. receive returned books
   5. check students’ record by student id or name
   6. check book rental record and storage (full list)

Extra (Not Implemented yet):

1. User function:
   1. add personal information
   2. upload avatar
2. Student function:
   1. expiring book alert
   2. buy book online
3. Staff function:
   1. sell book online