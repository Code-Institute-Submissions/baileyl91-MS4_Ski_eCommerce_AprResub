# Ski Shop

[View the live project here.](https:https://ski-ecommerce.herokuapp.com/)

This project was created as part of my Milestone Project 4 with Code Institute Web Application Development course.

For the project and to demonstrate what I have learned in the course, we needed to create an e-commerce store and have decided to create a ski shop.
The main goal of the website is to be an online shop for skiers to buy ski equipment.

## User Stories

Client Goals

* The site needs to be easily accessible.
* The navigation menu needs to be simple to use on a range of devices, including desktop, tablet and mobile.
* Navigating around the site should be simple and straightforward.
* The ability to register for an account, login and logout.
* The text should be clear to read.
* The images should be clear, not stretched and/or squashed.

First Time Visitor Goals

* The site should be easy to understand.
* The site should be easy to understand how to navigate through the site.
* A user should be able to create an account easily.
* The content should be clear and easy to understand.
* The checkout process should be straightforward and easy to understand.

Returning User

* Should be able to login.
* Be allowed to view previous orders.
* Should be able to purchase with previous saved details.
* Should be able to contact with website with any inquiry they have.

Admin User

* Should be able to create an account.
* Should be able to add a product.
* Should be able to edit a product.
* Should be able to delete a product.

## Design

**Color Scheme**

The colour scheme selected for the website is to reflect bluebird days when skiing. The nav bar and the footer would be a dark shade of blue with white text to represent the snow.The body is a very light shade of blue.

![Colour Pallete](static/docs/images/pallete.pdf)

**Typograpghy**

The main font I have used is the ‘Lato’ for its clean and minimal look with the backup font as sans-serif font if there were any problems using the first choice.

**Imagery**

The images for the hero carousel on the home page was sourced from Unsplash. The images chosen to show what the website is about but also to give visual clue as where the button directed to if user click on the button.

**Database Structure**

Database schema which can be viewed [here](static/docs/database/Database%20ER%20diagram%20(crow's%20foot).png)

**Wireframes**

Both desktop and mobile view

* [Home](static/docs/wireframes/Home%20Page%20Desktop.png)
* [Products](static/docs/wireframes/Products.png)
* [Product Detail](static/docs/wireframes/Products%20Details.png)
* [Checkout](static/docs/wireframes/Checkout%20Form.png)

## Features

There are a number of features that have been implemented into the website which are:

* Nav bar to allow users to navigate through the site
* Footer to store social media link
* Login into their account
* Social media links to connect users to the site social media
* Responsive on all devices
* Search bar 
* Register to create an account
* Users can log in to see their profile
* On profile page, users can see their order history
* Users can store their details for future purchases
* Users can edit their details in the profile page
* Users can view the products for sale 
* Users can sort through the products by A-Z, Name, Price and Category
* Users are able to click on the product to view more detail
* Users are able to pick a size and quantity 
* Users are able to add product to shopping basket
* Users are able to adjust quantity items in basket
* Users are able to see delivery cost and total cost of the basket
* Admin users are able to add, edit and delete a product

**Future Features**

* User can delete their own account
* Reviews for the products
* Review rating for the products
* Pagination for the products page

## Technology Used

**Language Used**

* HTML5
* CSS3
* JavaScript
* Python

**Frameworks, Libraries, and Programs Used**

* [Google Font](https://fonts.google.com/)
    * The font 'Lato' was imported from Google Font.
* [Font Awesome](https://fontawesome.com/)
    * Used to get some icons for the site.
* [Gitpod](https://www.gitpod.io/)
    * Gitpod is the development environment used to develop the project.
* [GitHub](https://github.com/)
    * GitHub is used to store the code for the site.
* [Git](https://git-scm.com/)
    * Git was used as version control, to add, commit and push Git and GitHub.
* [Balsamiq](https://balsamiq.com/)
    * Used to create wireframes for the website.
* [Google Developer Chrome Tools](https://developers.google.com/web/tools/chrome-devtools)
    * Used to inspect elements of the page and debug any potential problems within the website.
* [Unsplash](https://unsplash.com/)
    * Used to get stock-free images for the project.
* [Bootstrap](https://getbootstrap.com/)
    * Used to create a responsive site.
* [jQuery](https://jquery.com/)
    * Used to work with Materialize framework
* [Jinja](https://jinja.palletsprojects.com/)
    * Used as a templating language for Python to display backend data to HTML.
* [Coolors](https://coolors.co/)
    * Used to create a cohesive color scheme for the website.
* [Heroku](https://www.heroku.com/)
    * Used to deploy the website.
* [Django](https://www.djangoproject.com/)
    * Application framework.
* [AWS](https://aws.amazon.com)
    * Cloud application to hold media files

 ## Issues

 ## Testing

[Click here to see the testing documentation](TESTING.md)

## Deployment

**Deployment to Heroku**

1. Set Up A New Heroku App
    * Navigate to Heroku.com, create a new account, or log in if you already have an account.
    * On the dashboard page, click the "Create New App" button.
    * Give the app a name, the name must be unique with hyphens between words.
    * Set the region closest to you, and click "Create App".
2. Create A Requirements.txt file
    A requirements.txt file contains a list of the Python dependencies that our project needs to run successfully. It's how Heroku can detect what language we're using. Here are the steps to create a requirements.txt file:
    
    Create a requirements.txt file by typing in the terminal:
    ```
    pipi3 freeze --local > requirements.txt
    ```

    Add, commit, and push the file:
    ```
    git add -A
    git commit -m "Add requirements.txt" 
    git push
    ```
3. Create A Procfile file
    A procfile is a special kind of file that tells Heroku how to run our project.
    In the terminal, type:
    ```
    echo web: python run.py > Procfile
    ```

    This command tells Heroku that it's going to be a web process, and the command to run our application is "python run.py", which is the name of the python file that we've created.

    Add, commit, and push the file:
    ```
    git add -A
    git commit -m "Add Procfile" 
    git push
    ```
4. Connect Our App to Github
    * In the Heroku app dashboard, navigate to the Deploy page. On the Deployment Method, click "Github".
    * Click on the "Connect to Github" button.
    * Fill in the name of your Github repository name and click on "Search".
    * After it found the correct repository, click on "Connect".

5. Set Up The Environment Variables in Heroku
    Since we've contained our environment variables within a hidden file env.py, Heroku won't be able to read those variables. We can securely tell Heroku which variables are required.
    * Go back to the Heroku dashboard of your django app, navigate to the "Settings" page.
    * Click on the "Reveal Config Vars" button, add environment variables.

6. Enable The Automatic Deployment
    * On the "Automatic Deploys" section, from our master/main branch click on "Enable Automatic Deployment".
    * On the "Manual deploy" section, from our master/main click on "Deploy Branch".
    * Heroku will now receive the code from Github and start building the app using our required packages. Once it's done, you'll see a notification "Your app was successfully deployed." The deployed version can now be viewed by selecting View App.

**Forking the GitHub Repository**

By forking the GitHub Repository we make a copy of the original repository on our GitHub account to view and/or make changes without affecting the original repository by using the following steps.
1. Log in to GitHub and locate the GitHub Repository
2. At the top of the Repository (not top of page) just above the "Settings" button on the menu, locate the "Fork" button.
3. You should now have a copy of the original repository in your GitHub account.

**Making a Local Clone**

1. Log in to GitHub and locate the GitHub Repository
2. Below the settings, click on "Code".
3. To clone the repository using HTTPS, under "Clone with HTTPS", copy the link.
4. Open Git Bash
5. Change the current working directory to the location where you want the cloned directory to be made.
6. Type git clone, and then paste the URL you copied in Step 3.
7. Press Enter. Your local clone will be created.

## Credits

**Code**

To create the ski shop, I have relied heavily on the Boutique Ado
project.

**Content**

The content on the homepage was written by me.
The content for the products was taken from Snow & Rock website
 

**Media**

The hero images for the carousel was found on Unsplash, was created by [Maarten Duineveld](https://unsplash.com/photos/pmfJcN7RGiw), [Jeremey Bezanger](https://unsplash.com/photos/jW1I1M9TdRA) and [Ethan Walsweer](https://unsplash.com/photos/weFx9RflIfU).

The images provided for the products was taken from the [Snow & Rock website](https://www.snowandrock.com/).
A backup image for the products if there no image found was from Boutique Ado project.


**Acknowledgments**

Want to thank the Student Care and fellows students for their support. Also the tremendous community on the Slack channel.
Also wanted to say a massive thanks to Christine from tutor support for actually spending the whole morning debugging the issue with Heroku and AWS.
