# Less basics

[Learn Less in less than 10 mins](http://tutorialzine.com/2015/07/learn-less-in-10-minutes-or-less/)

## Variables

+ Use **@[variableName]:[value]** to define a variable




## Mixins

+ LESS enables us to use an existing class or ids and apply all it’s styles directly to another selector.
+ If you don’t want the mixin to appear as a rule in the CSS you can place parentheses after it
+ mixins can also receive parameters

```
#circle(){
  background-color: #4CAF50;
  border-radius: 100%;
}

#small-circle{
  width: 50px;
  height: 50px;
  #circle
}

#big-circle{
  width: 100px;
  height: 100px;
  #circle
}

```


**How maxin receive parameters**
```
#circle(@size: 25px){
  background-color: #4CAF50;
  border-radius: 100%;

  width: @size;
  height: @size;
}

#small-circle{
  #circle
}

#big-circle{
  #circle(100px)
}

```

## Nesting and Scope
