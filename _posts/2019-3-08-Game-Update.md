---
layout: post
title: "Game Update"
date: 2019-03-08
---
https://www.wescheme.org/view?publicId=3ZWkQaPxZ3

The title of the game is called Slime Game. The game is about you, a slime monster, going around and collecting slime balls, you lose points if you make contact with fire. The setting is a plain field out in the open. An example of a function in my game is the collide? function. 

; collide? : Number Number Number Number -> Boolean 
; How close is close enough?  
; We have the player's x and y, and a character's x and y.
; We can ask how far apart they are.  Did they collide?
; EXAMPLEs:

(define (collide? px py cx cy)
  (<=(distance px py cx cy) 67))
(EXAMPLE(collide? 1 2 3 4) (<=(distance 1 2 3 4) 67))
(EXAMPLE(collide? 5 6 7 8) (<=(distance 5 6 7 8) 67))
What each line does is,
Line 1: The contract for the collide? Function.
Line 2: Giving a hint about what you need for the collide? function.
Line 3: The variables of the function, collide?
Line 4: Asks a question did they collide?
Line 5: Examples
Line 6: The definition, or the header of the functions defines collide? With the variables, px py cx cy
Line 7: The second part of the definition, provides the example of the function collide? And the distance that is needed for two or more objects to collide.
Line 8: One of the example for the collide? Function. 
Line 9: Another example of the collide? Function.
Lastly, the role of the collide? function is to help two objects to be able to collide, and give points, or lose points. This function is what helps the game become a game by giving it the essential, reward, (slime balls) and danger (fire) to play a game. 
