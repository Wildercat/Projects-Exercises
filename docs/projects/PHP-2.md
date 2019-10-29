# PHP (Pretty Hefty Payload) Part 2 - Parser

### Description

Create a webpage that displays json that has been cleaned up for user viewing

For this project we will be using PHP to perform a GET request and parse data to the screen

### Table of contents

<!--ts-->

- [Project/Exercise Name](<#PHP-(Pretty-Hefty-Payload)-Part-2---Parser>)
- [Description](#Description)
- [Table of Contents](#table-of-contents)
- [MVP (Minimum Viable Product)](#MVP)
  - [Wireframe](#Wireframe)
  - [Tech Stack](#Tech-Stack)
- [Process](#process)
  - [Setup](#Setup)
  - [Application File Structure](#Application-File-Structure)
  - [Develop](#Develop)
  - [Deploy](#Deploy)
- [Requirements](#Requirements)
  - [Additional Requirements](#Additional-Requirements)
  - [Stretch Goals](#Stretch-Goals)
- [Additional Resources](#Additional-Resources)
  <!--te-->

### MVP

By default, the app should GET JSON data from the internet to your machine

#### Wireframe

![wireframe](../wireframes/api-php-1.png)

#### Tech Stack

1. PHP

### Process

##### Setup:

1. [Create GitHub repo (either online or locally)](../git-instructions.md), for example: `my-app`
2. Create necessary files for application and view in VS Code
   - Run shell script to expedite process unless you are using a framework
   - _If you are using a framework, disregard the "Application File Structure" section_
3. Import and route necessary css/js files (E.g. Bootstrap)
4. Save all and create your first commit to `master`, **then** switch to a dev branch

###### Application File Structure

Minimally:

```
web/
    index.php - main page
README.md - any important information
.gitignore - file that omits any directory/file from being tracked
```

Additional pages will be relative to the index.html file.

It is okay if your project has more files and directories, but you at least need the ones listed above.

##### Develop:

1. Create a `dev` branch to commit your code to
2. View changes and test locally
3. Save often, and commit to your development branch on GitHub when important changes happen
4. Push your commits to GitHub remote
5. For bug fixes, refactored code, and feature branches, you must create a branch off of `dev` onto a `new-feature` branch and create a PR into dev when complete

##### Deploy:

1. Create a Pull Request from `dev` into `master`
2. Confirm code is up to date and works correctly
3. Post links to your GitHub repo to the Projects Slack channel

---

### Requirements

To complete the assignment, you must complete the following:

1. Your PHP project part 1 will become a basic client CRUD app instead of looking at its own data. It will run on `localhost:3000` via `php -S localhost:3000`.
2. This new PHP project part 2 will exist in a seperate folder and run on MAMP to host MySQL on `localhost:8080`.
3. You will have 2 servers in seperate folders running at once. One to store the data in a MySQL server, and one to perform CRUD actions and display data.
4. Install [Allow CORS Google Chrome Plugin](https://chrome.google.com/webstore/detail/allow-cors-access-control/lhobafahddgcelffkeicbaginigeejlf?hl=en) to allow communication across multiple servers.
5. For the database server, you will create a PHP script for one of your servers that handles CRUD functions and emits data via json_encode() and recieves data via json_decode().
6. For the data viewer server, you can display the data how you wish, ideally display the raw data on screen to confirm it works (do not skip this step, very important)
7. Next, parse the raw data and create a basic form interface.
8. Perform CRUD actions on data ([POST, GET, PATCH, DELETE, etc.](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods)) and update the data on the  database server via POST.
9. Confirm database server is indeed updated when client server updates

#### Additional Requirements

- Website must be responsive
- Style your app as you wish
- Use the tools and technologies covered in class to complete your website. To see what we have covered, check the [Class Resources Repo](https://github.com/bootcamp-students/Resources).
- Your repo should be public so that others can see your code and comment on it.
  - _**Remember to push to GitHub!**_
  - Potential employers will view your GitHub profile, so activity is crucial!

#### Stretch Goals

- Create a flow diagram for the backend architecure to be used in an MVP
- Use API credentials to only allow access to users with an API key
- [Use reactstrap to dynamically display data in table](http://reactstrap.github.io/components/tables/)

#### If you finish early...

1. Continue to add your own content, additions, and pages to your site and improve the styling.
2. Add info to your projects README.md [README.md Best Practices](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
3. Add links and resources from this week to the [Class Resources Repo](https://github.com/bootcamp-students/Resources) by forking the repo and then initiating a pull request with your additions to the .md file.

### Additional Resources

- Ask questions :-)
- [Class Resources Repo](https://github.com/bootcamp-students/Resources)
- Learn more about [Good GitHub Practices](https://guides.github.com)
- [Learn PHP](https://www.w3schools.com/php/)

For more information about **_doing something_**, see these articles:

- [Why use a Database?](https://softwareengineering.stackexchange.com/questions/190482/why-use-a-database-instead-of-just-saving-your-data-to-disk)
- [SQL Injection 1 (video)](https://www.youtube.com/watch?v=ciNHn38EyRc)
- [SQL Injection 2](https://stackoverflow.com/questions/60174/how-can-i-prevent-sql-injection-in-php?rq=1)
- [SQL Good Queries](https://www.datacamp.com/community/tutorials/sql-tutorial-query)
