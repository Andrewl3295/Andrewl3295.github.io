---
layout: post
title: "Andrew Li, Weekly Reflection-13"
date: 2018-12-14
---

This week, we were doing a flag project. We were assigned flags, to create using code. The flags we create have to be geometrically correct, the same colors, and has to be scale able. Throughout this week I have completed some parts of my flag such as the shape, the pattern and finding and imputing the correct colors into the program. Some challenges that I faced was finding and doing the correct dimensions along with making it scale . Which I didn't do yet. Some questions I had was how to add a custom color to the program and use it, and how to create a radio-star and a crescent. We were given information on how to make the flag scale able. We had to replace specific numbers with HEIGHT, WIDTH, or STRIPES. Then we can define those to make it a value that we can multiply. You can do make-color, and put in the rgb of the color that you want, then define it to be able to use that color. 













```
;colors of the flag;ratio 1:2
;colors of the flag
(define color-blu (make-color 1 0 102))
(define color-re (make-color 204 0 1))
(define color-yello(make-color 255 204 0))
;Words to replace numbers
(define WIDTH(* 400))
(define HEIGHT(* 200))
(define 1/2HEIGHT(* 100))
(define stripehight (* 14))
;simple shapes of the flag
(define x(rectangle WIDTH HEIGHT "solid" "white"))
(define y(rectangle HEIGHT 1/2HEIGHT "solid" color-blu))
(define cre(rotate 30 (put-image(circle 50 "solid" color-blu) 55 35 (circle 55 "solid" color-yello))))

(define base (put-image (rectangle HEIGHT 1/2HEIGHT "solid" color-blu) 100 150 (rectangle WIDTH HEIGHT "outline" "gray")))
(define crecent (rotate 360(put-image(circle 32 "solid" color-blu) 42 35 (circle 35 "solid" color-yello))))

(define bc (put-image crecent 86 150 base))

(define redstripes (rectangle WIDTH stripehight "solid" color-re))
(define redBase1 (put-image redstripes HEIGHT 79 bc))
(define redstripeshalf (rectangle HEIGHT stripehight "solid" color-re))
(define a (put-image redstripeshalf 300 193 redBase1))
(define b (put-image redstripeshalf 300 164 a))
(define c (put-image redstripeshalf 300 136 b))
(define d (put-image redstripeshalf 300 107 c))
(define f (put-image redstripes HEIGHT 51 d))
(define g (put-image redstripes HEIGHT 23 f))
(define starr (scale 0.6 (star 14 22 50 "solid" color-yello)))
(define flag-m (put-image starr 120 150 g))
flag-m
```

![Flag Screenshot](/images/FlagV2.png)
