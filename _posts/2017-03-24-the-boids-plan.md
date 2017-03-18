---
layout: post-sidebar
title: "Boids: planning the project"
date: 2017-03-24 11:54:26
categories: dsp2017
author_name : Kamila
author_url : /author/kamila
author_avatar: kamila
show_avatar : true
read_time : 10
feature_image: feature-plan
show_related_posts: true
comments: true
square_related: recommend-plan
---
<br>
<blockquote>
    <p><em>Failing to plan is planning to fail.</em></p>
    <footer>Alan Lakein</footer>
</blockquote>
<br>

Before I decided to register to the “Get Noticed” contest, I had read a whole bunch of posts and articles by attendees of the 2016 edition. They were describing how the participation itself helped them grow as developers, why it is all worth time and effort - and how to prepare yourself to the challenge. Not surprisingly, they all emphasised the significance of having a good, thoughtful plan, factorizing the problem and getting into details of every single step. With that in mind, I started coding with… several sheets of paper and tons of bookmarks open in my browser to analyze what actually needs to be done and how to start. Here is what I have come up with.

## Stage 1: Choosing tools and technologies

This one was quite obvious: HTML & CSS(Sass) for the project’s shell, JavaScript for the engine. Since there are many cool features introduced by ECMAScript 2015 (wider known as ECMAScript 6 or simply ES6), I will try my first steps here, taking advantage of the newly introduced classes, arrow functions, destructuring etc. The Boids themselves will be animated on HTML5 canvas and I plan to prepare an introduction to the canvas API in the nearest future.

## Stage 2: Preparing the environment

Another warm-up thing: preparing a visual platform at which Boids will be flying. I have created a palette of swatches (an old designer’s habit) and decided to divide the layout vertically, leaving a left-hand aside for some basic information on the Boids idea and a simple manual. All the rest will be taken up by canvas. Initially I wanted to start with a single bird-oid form animating itself but then I changed my mind and chose a roughly straightforward solution to begin with. The elementary Boids will be simply small circles drawn directly on canvas. Once I figure out all the animation’s algorithms, I will try to think of a way to turn circles into something more complex. First things first.

## Stage 3: Maths!

Now here comes the hardest thing for me, or at least at this point it seems so. Getting into counting! Vectors, numbers, algorithms… putting together three seemingly simple rules of flocking put me hardly off. Still, it had to be done. OK, a pile of blank paper sheets and a pen and let’s dismantle the sucker!

I will need a 2D coordinate system and an array of starting positions of Boids (x and y). Thereafter, Boids will be placed on the given coordinates and put into motion. At this point there has to be a function that takes the initial coordinates and counts the next position of each boid as per the rules described in the former post. A quick reminder:

+ **separation**: steer to avoid crowding
+ **alignment**: steer towards the average heading of local flockmates
+ **cohesion**: steer to move toward the average position of local flockmates

Let’s break these apart.

## Stage 4: Creating a Boid class

## Stage 5: Initial animation for a group of Boids

## Stage 6: Counting next position

## Stage 7: Changing the circle into bird-oid form

## Stage 8: Adding controls

## Stage 9: First roadblock

## Stage 10: Dynamic roadblocks on user’s click

## Stage 11: Getting it nice!

