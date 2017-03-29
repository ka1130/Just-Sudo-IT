---
layout: post-sidebar
title: "8 ES6 features I use in the Boids project (and work great anywhere!)"
date: 2017-04-19 09:00:12
categories: dsp2017 coding
author_name : Kamila
author_url : /author/kamila
author_avatar: kamila
show_avatar : true
read_time : 30
feature_image: feature-es6
show_related_posts: true
comments: true
square_related: recommend-es6
---
The introduction of ECMAScript 2015 standard, also known as ES6, is a quantum leap for JavaScript that the language hadn’t seen since 2009. I didn’t realize the significance of the changes until very recently when I started to learn the new ES6 features. Some of them are pretty self-explanatory, the others took me more time to comprehend - and there’s still a bunch of stuff I have only blurry idea about. Since the best way of learning to code is actually… to code, I decided to introduce ES6 to the Boids project. And you know what, it considerably simplified and clarified the work. So I decided to share some insight with you. Here are the 8 ES6 features I have used when programming Boids.

## 1. Block-Scoped Constructs: Let and Const

ES6 has introduced two new ways of defining variables. Apart from `var` we have also now `let` and `cost`. Now what are `let` and `const` for and why was `var` not enough? 

The main problem with `var` was its scope, which is a function scope, whereas `let` and `const` are block-scoped. It means they only exist within the current block represented by a pair of curly braces: `{}`: it may be a block within an `if` statement, a loop - or you can simply create one and put your `let` or `const` inside. This helps avoid common developers’ problems and makes JavaScript behave more predictably to those used to work in other languages, such as Java, C or C++.

Also, when using `let` and `const` you do not fall into the hoisting trap, which you may welcome with relief as many people find the hoisting idea pretty distressing. This is because `let` and `const` remain uninitialized until they are declared. The timespan before `let` or `const` initialization is called “Temporal Dead Zone” (TDZ). For more in-depth explanation, have a look [here](https://ponyfoo.com/articles/es6-let-const-and-temporal-dead-zone-in-depth).

Next, `let` and `const` declarations cannot be reassigned. So you won’t accidentally overwrite your variables. You can only update the value of `let`. By contrast, `const` declaration is created to keep values that will not be changed. Some programmers say it’s best to use `const` by default and `let` only in special cases, when the value of the variable is bound to be changed (such as the counter in your `for` loop).

Last but not least, `let` and `const` do not become properties of the global object, in case you defined them globally (which you should never do by the way). The same is true for the new ES6 Classes - and I’ll tell you more about them later in this post.

Of course, you can still use `var` if you want, there's nothing wrong with that. Just be aware of it's characteristics and give the new constructs a try too see if you feel commfortable working with them.

## 2. Arrow Functions

A cool new feature of ES6 are arrow functions, also referred to as fat-arrow functions. Their name stems from the token they use: `=>` which looks… well, like a fat arrow. Arrow functions are just a more concise syntax for writing function expressions. They also handle `this` bindings in functions in a bit different way.

## 3. Default Parameters


## 4. Template Literals 


## 5. Array Helpers


## 6. Rest & Spread Operators


## 7. Destructuring


## 8. Classes


## Babel


## Summing Up & Learning Resources

