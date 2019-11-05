# Laravel Library

### Description

Create a webpage that acts as a hub for librarians to know the status of books in their library, and update books and their information

For this project we will be using Composer to generate a Laravel project, and adding an artisan preset to use React.js in our laravel project to create components to put onto blade.php files

You will not be able to host this site on github, but you will still store github versioning online, so to learn about how to properly [link a repo created on the command line with an existing repo you created on the GitHub website, click here](https://help.github.com/en/articles/adding-an-existing-project-to-github-using-the-command-line)

For site hosting, we will be using Google Cloud

### Table of contents

<!--ts-->
- [Project/Exercise Name](#Laravel-Library)
- [Description](#Description)
- [Table of Contents](#table-of-contents)
- [MVP (Minimum Viable Product)](#MVP)
  - [Wireframe](#Wireframe)
  - [Tech Stack](#Tech-Stack)
- [Process](#process)
  - [Setup](#Setup)
  - [Develop](#Develop)
  - [Deploy](#Deploy)
- [Requirements](#Requirements)
  - [Additional Requirements](#Additional-Requirements)
  - [Stretch Goals](#Stretch-Goals)
- [Additional Resources](#Additional-Resources)
<!--te-->

### MVP

By default, the app should let a Librarian maintain a simulated library via a web interface which communicates with the Google Books API to populate book content.

#### Wireframe

[Library Wireframes](../wireframes/library) - you do not need to copy these exactly, it's just one of many ideas.
Remember, this is a back end project; it does not need to look pretty, it needs to work. You can use React.js to play around in the front end, but only after you get it working behind the scenes.

#### Tech Stack

1. HTML
2. CSS
3. JS
4. React.JS
5. MySQL
6. PHP
7. Laravel

### Process

##### Setup:

1. [Create GitHub repo online](../git-instructions.md), for example: `laravel-library`
2. Create necessary files for application and view in VS Code via `laravel new library` 
3. Import and route necessary css/js files (E.g. Bootstrap)
4. Save all and create your first commit to `master` , **then** switch to a dev branch

##### Develop:

1. Create a `dev` branch to commit your code to
2. Add content and elements to your website
3. View changes and test locally
4. Save often, and commit to your development branch on GitHub when important changes happen
5. Push your commits to GitHub remote
6. For bug fixes, refactored code, and feature branches, you must create a branch off of `dev` onto a `new-feature` branch and create a PR into dev when complete

##### Deploy:

1. Create a Pull Request from `dev` into `master` 
2. Confirm code is up to date and works correctly
3. Post links to your GitHub repo to the Projects Slack channel

---

### Requirements

*Do not begin using React.js until you have successfully completed the project. This is a back end project; it does not need to look pretty, it needs to work.*

To complete the assignment, you must complete the following:

1. Store a table of library card holders as `users` in your local MySQL database.
2. Use the [Google Books API](https://developers.google.com/books/docs/v1/getting_started) to generate book content for users to check in and out from the library and to store a table of fetched books as `books` in your local MySQL database. This data should only be updated/fetched as the superuser Librarian
3. Store a table of checked out books and meta data such as date and number of times checked out as `checkouts` in your local MySQL database.
3. Implement full CRUD operations.
4. Implement foreign key relations to correctly store data
5. Use React.js for creating components to put on Laravel Blades.
6. Users do not *need* to sign up or be real people, you can simulate this by clicking a "new user" button in the admin interface as a Librarian.
7. Show all user and book statistics that are saved in database (for example: There are 3 users registered with the library, user "jim" has 2 books checked out: "Algorithms", and "Design Patterns", user "phil" has 0 books checked out, and user "sally" has 1 book checked out: "The Pragmatic Programmer", there are 5 books in the library total, three are checked out, etc.) you can format this data however you'd like, we suggest a html table with multiple tabs
8. Be able to click any user or book and view the info as well as perform full CRUD where applicable.(librarian superuser can perform any action and view any page, but basic card holder user can only view a subset of pages and perform limited actions)
---
* To [set up React.js into Laravel](https://dev.to/lvtdeveloper/using-react-in-a-laravel-application-8fp)

1. `laravel new laravel-library` 
2. `cd laravel-library` 
3. `php artisan preset react` 
4. `npm install && npm run dev` 

**Do not begin using React.js until you have successfully completed the project. This is a back end project; it does not need to look pretty, it needs to work.**

#### Additional Requirements

* Website must be responsive
* Style your app as you wish
* Use the tools and technologies covered in class to complete your website. To see what we have covered, check the [Class Resources Repo](https://github.com/bootcamp-students/Resources).
* Your repo should be public so that others can see your code and comment on it.
  + _**Remember to push to GitHub!**_
  + Potential employers will view your GitHub profile, so activity is crucial!

#### Stretch Goals

* Create backend archetecture wireframes for use in a potential MVP
* Create a search bar for querying books from the Google Books API
* Create a full stack site by [using React.js for all front end](https://dev.to/lvtdeveloper/using-react-in-a-laravel-application-8fp)
* Implement Laravel Auth using composer to create many "Librarians"
* Add a 'due by date' that keeps track of how long a book has been checked out
* Add a 'late fee' for books that have been checked out too long that can be modified by the librarian
* Add a way for a user to 'renew' their checked out book
* Add a way for users to put a book on hold if someone else has it currently checked out
* Add a history for the librarians to see a list of all people who checked out a particular book
* Add any other data to the scheme as long as it is NOT redundant
* [Use React.js as a frontend that communicates with the Laravel library as a REST API](https://restfulapi.net/)

#### If you finish early...

1. Continue to add your own content, additions, and pages to your site and improve the styling.
2. Add info to your projects README.md [README.md Best Practices](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
3. Add links and resources from this week to the [Class Resources Repo](https://github.com/bootcamp-students/Resources) by forking the repo and then initiating a pull request with your additions to the .md file.

### Additional Resources

* Ask questions :-)
* [Class Resources Repo](https://github.com/bootcamp-students/Resources)
* Learn more about [Good GitHub Practices](https://guides.github.com)

For more information about CRUD, see these articles:

* [What is CRUD?](https://www.codecademy.com/articles/what-is-crud)
* [Why is CRUD so Important?](http://trendintech.com/2018/01/19/why-is-crud-so-important-in-computer-programming/)

Using React with Laravel

* [Putting React.js into Laravel](https://dev.to/lvtdeveloper/using-react-in-a-laravel-application-8fp)

