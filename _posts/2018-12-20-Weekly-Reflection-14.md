---
layout: post
title: "Flag Project - Final Submission"
date: 2018-12-20
---

## Flag of Malaysia by Andrew Li

## Describe your program

  The country that I designed for was Malaysia, which is in Asia. The grade that I expect is a 4, because I chose the "harder" flag, and yet met all the requirements for completeing the project. 

## Current output

* * *
![Flag](/images/final-flag.png)
* * *

## Describe your process.

Some questions that I had was how to create ceartian shapes of the flag, such as the radio star, and the crecent, but I overcome that by getting help by my peers, that help me by telling me the process of how to create those shapes. Some stragtegies that I used was none. I just worked in class and completed it.

## Explain your code.

* * *
So the lines that I submitted are the lines that makes up the red stripes of the Malyasia Flag. What I did was define each stripe by the alphebelt, that used that and ekpt on going on, I subtraced each stipe by a constant number, to make it correct. How it works by itself, is that is shows that stripes by itself,then all together, how it is within the whole program is that it gives it the vibe of the Malyaisa Flag. 

```
(define redstripes (rectangle WIDTH stripehight "solid" color-re))
(define redBase1 (put-image redstripes HEIGHT (* size 79) bc))
(define redstripeshalf (rectangle HEIGHT stripehight "solid" color-re))
(define a (put-image redstripeshalf stripex (* size 193) redBase1))
(define b (put-image redstripeshalf stripex (* size 164) a))
(define c (put-image redstripeshalf stripex (* size 136) b))
(define d (put-image redstripeshalf stripex (* size 107) c))
(define f (put-image redstripes HEIGHT (* size 51) d))
(define g (put-image redstripes HEIGHT (* size 23) f))
(define starr (scale 0.6 (star 14 (* size 22) (* size 50) "solid" color-yello)))
(define flag-m (put-image starr (* size 120) (* size 150) g))
flag-m

```

* * *

-   Explain the code you posted by telling us about each argument.
-   Then tell us how your code section fits into the whole.
The code I posted was my code for the Malaysia Flag, the beggining part was the definitions, of the Malyaisa Flag. Such as the colors, and width and height, as well as the stripes, and colors of the flag. After that is the simple shapes of the flag, this part contains the simple shapes, such as the rectangles. Next is creating the base of the flag, I used a rectangle, then used put images, to place images on top of each other to get the flag. Then the last part of the program, is that creation, and making ofthe stripes of the Malaysai Flag. I came up with the numbers by finding a common number with the width and height. Then I did the greatest common factor of all the numbers to be able to scale, and got 1.

## Program code

```
;colors of the flag;ratio 1:2
;colors of the flag
(define color-blu (make-color 1 0 102))
(define color-re (make-color 204 0 1))
(define color-yello(make-color 255 204 0))
;Words to replace numbers
(define size 1)
(define WIDTH(* size 400))
(define HEIGHT(* size 200))
(define 1/2HEIGHT(* size 100))
(define stripehight (* size 14))
(define stripex (* size 300))
;simple shapes of the flag
(define x(rectangle WIDTH HEIGHT "solid" "white"))
(define y(rectangle HEIGHT 1/2HEIGHT "solid" color-blu))
(define cre(rotate 30 (put-image(circle 50 "solid" color-blu) 55 35 (circle 55 "solid" color-yello))))

;Putting the Flag Together
(define base (put-image (rectangle HEIGHT 1/2HEIGHT "solid" color-blu) 
                        (* size 100) (* size 150) (rectangle WIDTH HEIGHT "outline" "gray")))
(define crecent (rotate 360(put-image(circle (* size 32) "solid" color-blu) (* size 42) (* size 35) (circle (* size 35) "solid" color-yello))))

(define bc (put-image crecent (* size 86) (* size 150) base))

;Making of the stripes
(define redstripes (rectangle WIDTH stripehight "solid" color-re))
(define redBase1 (put-image redstripes HEIGHT (* size 79) bc))
(define redstripeshalf (rectangle HEIGHT stripehight "solid" color-re))
(define a (put-image redstripeshalf stripex (* size 193) redBase1))
(define b (put-image redstripeshalf stripex (* size 164) a))
(define c (put-image redstripeshalf stripex (* size 136) b))
(define d (put-image redstripeshalf stripex (* size 107) c))
(define f (put-image redstripes HEIGHT (* size 51) d))
(define g (put-image redstripes HEIGHT (* size 23) f))
(define starr (scale 0.6 (star 14 (* size 22) (* size 50) "solid" color-yello)))
(define flag-m (put-image starr (* size 120) (* size 150) g))
flag-m
```
