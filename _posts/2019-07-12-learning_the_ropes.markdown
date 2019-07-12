---
layout: post
title:      "Learning the Ropes"
date:       2019-07-12 21:16:57 +0000
permalink:  learning_the_ropes
---


Having recently finished my very first CLI project, I’ve learned very valuable lessons that will enhance my coding skills in the months to come.  When first approaching the project, I knew right away I wanted to showcase my love for coffee and appeal to the hearts of other caffeine addicts out there who needed coffee for survival!  In other words, I wanted to create something that I felt passionate about, and had experience with, or rather experience drinking.  Although creating my Virtual Café project started off as a fun adventure, there were definitely moments when I felt confused and doubtful about certain concepts.  One example of intense doubt and suffering was understanding how to efficiently deal with an if-else crisis.  Prior to refactoring I noticed that my code was overstuffed with if-else statements, and by no means was that a good look.  For example, within the CLI interface class, I had a user menu coded with 15 coffee drinks for the user to reference, (i.e. type 1 for “Frappuccino”) and each drink had an if statement before it (i.e. if input == “Frappuccino...”).  However, the real issue with the menu could be traced back to the scraper class--I had written the code for the scraper class correctly, but with little finesse.  I was making the scraper class responsible for returning *all *of the coffee drinks (using the if statements in the CLI interface to point to each one), instead of one individual instance of a coffee drink based on the user’s input.  Thanks to some additional help from my section coach, I was able to refactor my scraper class and eliminate unnecessary code within my CLI interface.  This isn’t to say that if-else statements are bad, in fact they’re remarkably useful; it just means that the best strategy is to simplify conditional statements when, and if possible, which improves readability and functionality.  

Another valuable lesson I learned was using higher level operators like the ternary operator to handle conditional statements.  A ternary operator consists of 3 operands that takes 3 arguments:  first, you supply an expression, and after the expression you supply 2 values of true and false.  One of those values will be executed upon evaluation of the initial expression.  For example, see the code below.
                                                              
																															` valid_coffee_input ? show_drink : invalid_response`
																																
In this code snippet, taken directly from my CLI interface, if the user enters the correct (valid) input (a number corresponding to a coffee drink) the first statement (true) will execute:  the show_drink method.  However, if the user enters an invalid character or word, the second statement (false) will execute:  the invalid_response method.  In this example, if-else statements don’t have to be utilized, which is a good way of simplifying and maintaining code.

All in all, I’ve learned a lot more than I’ve explained here, and although I can’t cover all of the lessons I’ve walked away with, I can definitely say that this project has enlightened me in new ways and has given me a much more profound understanding of what object oriented programming is really all about.



