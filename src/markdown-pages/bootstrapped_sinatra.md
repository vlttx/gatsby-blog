
---
title: "Adding Bootstrap to My Sinatra App"
date: "2019-11-05"
---

# Adding Bootstrap to My Sinatra App

For my Sinatra Project I created **a very bare-bones** Sinatra App that helps a user keep track of their clients and their info. Once my database was set up, relationships established, routes properly added, as well as login and other requirements were met, I decided to play around with Bootstrap for a bit and see if I could figure out how it works. 

Be aware that I have never used Bootstrap before, so I am sure that my way of doing things might not be the best way, but I did manage to add some random things to my app (I say random because I was just trying out whatever struck my fancy). 

First of all, I downloaded Bootstrap [here](https://getbootstrap.com/docs/4.3/getting-started/download/). Then, I created a separate folder for my soon-to-be bootstrapped app. I could have tried having a separate branch and then merging it into my master branch but I wanted to keep things as separate as possible in case I mess up. 

I created a folder "bootstrapped-client-tracker-app" and I copied all of my content from my original app folder into the new folder and then I took the unzipped Bootstrap folder and copied it into the **public/stylesheets** folder. Then, I finally created a separate repository and started experimenting.

I figured that I would need to include links to my bootstrap.css within the **layout.erb** template since that was the main template of my web app.  First of all, I deleted my main.css file and then, in my layout.erb file I made sure to link to my Bootstrap CSS instead. 

![](https://jh6b8g.bn.files.1drv.com/y4mR7lsk7mUY-ZRM-83I9DuEyw547-P2N5Ev5WhPHT6RqivqhmVEIF3eRp68UEnbUbDRr6MzOH2O0eiXyBxZ1q3rNM7yOyMfcA2NOLJfpNItLH4SMZVB3CxLAdS7pJQHk6j3n6R1_bpsDoUl3wCnIK77iCUT0YDRO6V8KMjwewRSEjKDRocOd3XfD9igbrF1MoJtS25cV9_NOtgXp7QFW6RNA?width=1044&height=598&cropmode=none)

Then, I started experimenting with various colors in order to see if all that CSS coming from Bootstrap will work on my app. I also tried to determine which container is where and whether it would make sense to edit its look. As you can see, I have added background-image to my body separately, as well as made my main text white because it took me forever to figure out where which container begins and where should I edit what in order to get the effects I wanted. Trying to edit the CSS provided by Bootstrap reminded me more of a detective work than anything else but it was definitely fun. 

The next thing I wanted to do was to add a navbar. I went to the checkout Bootstrap [Components/Navbar](https://getbootstrap.com/docs/4.3/components/navbar/) section
and applied the navbar code they provided. Of course, I customized it to fit my needs as I had my own pretty boring navbar already built, so now it was only the question of how nice I can make it look. 

![](https://i36b8g.bn.files.1drv.com/y4mk8HaQDBRJGW-YA3W4WwxkmNFMJLkIWIDE5jJI1MIq7K0G3WVEYL-4biQVZU8LsTrN-jElGzXMfKPYYV6TMORL52IUCoBDa89tIivF9cxo6OYWEBZ-Jf9uRN-zAoWnI_ubqw5vr7Pnf-wqD__0CLLI09dcqQwNDB_X7AwTtVu2E-v7RaHHjXxP9bpg_OQzjPz0XGHI4AsZqahMzKO-FXltw?width=1348&height=726&cropmode=none)

Another important part that I really wanted to change were the buttons. Mine were pretty ugly and I could not wait to make them look less like they were from a 90s website. Again, I looked under components and just copied the given CSS code that would provide me with the style I need. However, the only difference here was that I could not just apply CSS to my **layout.erb** and be done with it. I had to go to each view file where I had buttons and manually add the styling in order to make my web app have consistent colors. Here is an example of how my **login.erb** form code looked now:

![](https://i36b8g.bn.files.1drv.com/y4mk8HaQDBRJGW-YA3W4WwxkmNFMJLkIWIDE5jJI1MIq7K0G3WVEYL-4biQVZU8LsTrN-jElGzXMfKPYYV6TMORL52IUCoBDa89tIivF9cxo6OYWEBZ-Jf9uRN-zAoWnI_ubqw5vr7Pnf-wqD__0CLLI09dcqQwNDB_X7AwTtVu2E-v7RaHHjXxP9bpg_OQzjPz0XGHI4AsZqahMzKO-FXltw?width=1348&height=726&cropmode=none)

It is really not that difficult to divide your page into containers, rows and columns when you get a hang of it and get used to it. By the time I applied this style to all of my buttons, I started to understand how this grid/responsive system works and why it is so convenient. I became more aware of block elements and inline elements as well as general structure of a page.

This was just a glimpse of what I experimented with and what worked for me. I could have probably added more interesting styles in order to make my Sinatra app appear nicer but I know that Sinatra is just a stepping stone to Rails and that I will have many more chances to experiment with Bootstrap, so I did not invest too much of my time here. I feel like now I understand not only how the MVC architecture works but also have an idea how Bootstrap can make my web app look more colorful and fun. I did experiment a lot more with it than I am showing here but it was more for learning purposes than anything else, so there is not much that I can show. I can only encourage anyone who has no experience with Bootstrap and is thinking about trying out Bootstrap on their Sinatra app to just try it out. If I was able to add it and change the look of my app, so can you. Of course, Bootstrap provides a lot more than just navbars and buttons that I showed above but everyone has to start somewhere! :) 

