---
layout: post
title:  "Django GT Movies Store Application"
date:   2026-09-13
categories: Software #actually the description
#description: adfklja;dlkfj;
#permalink: /projects/:title
---
A web application that allows users to access information about movies and place orders to purchase them. Users are also able to list, create, edit, and delete movie reviews. Built using Django.

## Features

### General Pages
When a user first opens the website, they are greeted with the homepage.\
![The home page]({{"/assets/Screenshot2026-09-14121347.png" | relative_url }}){: width="500" }

Theres an about page that has information about the store so they can learn more about the app and its purpose.\
![The about page]({{"/assets/Screenshot2026-09-14123355.png" | relative_url}}){: width="500" }

The movies page lists the avaliable movies and they can be searched through using the search bar on top.\
![The Movies Page]({{"/assets/Screenshot2026-09-14121401.png" | relative_url}}){: width="500" }

Upon clicking on a movie, you get more information about it and are able to see user reviews and the movie to your cart to purchase.\
![The Avatar Page]({{"./assets/Screenshot2026-09-14121434.png" | relative_url}}){: width="500" }

### User accounts
Users can make accounts with the 'Sign Up' page and login using the login page. Creating an account allows users to make reviews and purchases.\
![The Sign Up Page]({{"./assets/Screenshot2026-09-14124805.png" | relative_url}}){: width="500" }
![The Login Page]({{"./assets/Screenshot2026-09-14124824.png" | relative_url}}){: width="500" }

### Reviews
Users can create, edit, and delete their own reviews. Users can also report other peoples reviews if they deem them to be inappropriate.\
In the image below, we are logged in, so we see the create review box and we can also report other peoples reviews.\
![Review Page]({{"./assets/Screenshot2026-09-14121503.png" | relative_url}}){: width="500" }

Here we made a review and you can see how for our own review, we have options to delete and edit it.\
![Added a review]({{"./assets/Screenshot2026-09-14121618.png" | relative_url}}){: width="500" }

If we choose to edit the review, we get to this website where we can make changes.\
![Edit a review]({{"./assets/Screenshot2026-09-14121659.png" | relative_url}}){: width="500" }

If we find an inappropriate review, we can report it so admin can take care of it (see Administration section). We don't want it to simply delete the review, because somone may abuse the system. Below is the dialog we see once we click "report".\
![Reported review]({{"./assets/Screenshot2026-09-14121714.png" | relative_url}}){: width="500" }

### Purchases
Users can add movies to their cart to purchase later.\
![Cart]({{"./assets/Screenshot2026-09-14121951.png" | relative_url}}){: width="500" }

Page when you click 'Purchase':\
![Completed order]({{"./assets/Screenshot2026-09-14122003.png" | relative_url}}){: width="500" }

Order page to see your orders:\
![Order pages]({{"assets/Screenshot2026-09-14122028.png" | relative_url}}){: width="500" }

### Administration
Site adminstrators complete access to create/view/edit/delete orders, movies, reviews, and users. Below is the main site administration page:\
![Admin page]({{"assets/Screenshot2026-09-14122312.png" | relative_url}}){: width="500" }

They can see and make changes to everything, but as an example, lets look at the reviews. When an admin clicks on "Reviews", they are greeted by a list of reviews, with each displaying its ID, Movie, and number of Reports. Notice that one review has a report.\
![Admin reveiws page]({{"assets/Screenshot2026-09-14122327.png" | relative_url}}){: width="500" }

If we click on one of these reviews, we can see the number of reports, the comment itself, the movie it's reviewing, and the user that posted it. As an admin, we are free to edit/delete reviews. In the case with the review below, it has been reported and is innapropriate so we can delete it.\
![Admin page]({{"assets/Screenshot2026-09-14122339.png" | relative_url}}){: width="500" }

## Process
This project served as an introductory project to learn Django. This project follows the process featured in the textbook "Django 5 for the Impatient : Learn the Core Concepts of Django to Develop Python Web Applications" by Dr. Daniel Correa and Mr. Greg Lim.

After installing the necessary programs, I started by implementing a base template and making the movie store with dummy data. At this point, no database functionality has been implemented.

Then, I began to implement the database by implementing user signup and login, letting users create, edit, and delete reviews, and allowing users to purchase movies and access order pages.

The "report reviews" features is not outlined in the process featured in the texbook, so I implemented it from scratch. I had many possible choices on how to implement it.\
I innitialy planned for it to simply be a button that all users could click (logged in or not), but I realized that a non-user may abuse the system, so I left the reporting functionality only to users.\
I innitialy implemented it with just a button press, but after using it, I realized that it wasn't clear that the report was actually processed. So, I made a page that confired that the report was made successfully and that admin would look at it.

## Video
Check out the video demonstration [here](youtube.com)!
