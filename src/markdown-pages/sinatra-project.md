---
title: "Building Client Tracker with Sinatra"
date: "2019-11-12"
---

### Client Tracker App with Sinatra

Since the day that I started freelancing, I always wanted to build myself a simple client tracker. That’s part of the reason why I started coding in the first place - I wanted to learn to make tools that make mylife easier. It is definitely part of my job to keep all my clients on file as there are hundreds of them that I encountered throughout my career and finding their business information easily is very important to me, so I built a web app where a user can safely log in and start creating lists of their clients and their information.

The greatest challenge when building this project for me was to set up correct associations and make sure all my routes work. Using Corneal definitely helped a lot. In order to keep my sanity, I decided to follow some good examples online and see whether I could build similar structures. I did not concentrate too much on HTML and CSS this time at all, as my main goal was to just make it work before worrying about the embellishments.

My main models for this project were User and Client models. I needed my users to be able to perform CRUD operations, have secure passwords and not be able to edit or delete other users’ clients. Eventually I made it so they would not be able to see other users’ clients at all. After creating these models and establishing their connections with each other, I created the database where their information was stored. The part that I liked the most was actually building routes and getting error messages when Sinatra would inform me that it does not know that ditty! It felt like Sinatra was a sort of puzzle generating machine and solving puzzles is really something I enjoy! It taught me a lot about how GET and POST requests are processed and what makes Sinatra work.

Even though my app right now is super simple, it does seem to work without any major hiccups whichever button I click, so that makes me happy. When I built my first CLI Gem Project, I also concentrated on predicting various user behaviors and making sure that it would not trap the user in a spot with no exit. Right now it seems like wherever my user ends up, they have a way out and that’s good, right?

I definitely wish my app was more visually appealing and much more complex than this but for now it will have to do. I have a lot of ideas as to how I could improve or what other apps I would like to build in order to make my freelancing life easier. Hopefully, my work will slow down soon and I can get back into the completely immersive experience that I had before.
