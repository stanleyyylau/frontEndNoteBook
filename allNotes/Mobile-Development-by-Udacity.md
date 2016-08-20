# Mobile web development

## Mobile UX

+ mobile default viewport to 980px
+ you can set viewport to a fix width
+ you can set viewport to **width=device-width**  == don't scale me bro

+ Bug: You can use Initial Scale, IOS will scale it in landscape mode if you don't set initial scale
you should set defualt font-size, bucase on IOS landscape mode, font-size will get scale, we recommand a reset
http://meyerweb.com/eric/tools/css/reset/


+ Mobile website starts with this magiccal tags
```
<meta name='viewport' content='width=device-width,initial-scale=1'>
```

+ on android device, set miniml and maximal scale to 1 for easy development, but dont do it on production

+ dont set User Scalable to no!!!

+ introducing viewport units http://beta.caniuse.com/#search=viewport

+ vmin and vmax for button creation

## Creating fluid layout

Learn flexbox on youtube

## Media query
+ device pixel ratio   dpp  http://stackoverflow.com/questions/31955113/what-is-different-between-devicepixelratio-and-dppx
+ web platform is lying
+ to get consistent experience, mobile device pass diffrent layout viewport to
+ divice inpendent pixel per inch  around 160m   Dots per inch (DPI)    Device-independent pixel (DIPs).  http://dpi.lv/
+ you can use ratio in media queries to controle background images
