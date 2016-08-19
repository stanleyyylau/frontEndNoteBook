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

+ Less nesting and Sass nesting is the same
+ Just like in programming languages, in Less variables receive their values depending on the scope.

```
@text-color: #000000;

ul{
  @text-color: #fff;
  background-color: #03A9F4;
  padding: 10px;
  list-style: none;

  li{
    color: @text-color;
    border-radius: 3px;
    margin: 10px 0;
  }
}

```


## Operations

+ You can do basic math operations to numerical values and colors.

```
@div-width: 100px;
@color: #03A9F4;

div{
  height: 50px;
  display: inline-block;
}

#left{
  width: @div-width;
  background-color: @color - 100;
}

#right{
  width: @div-width * 2;
  background-color: @color;
}

```


## Functions

+ Take a look at fadeout function, a function that decreases the opacity of a color.
+ **&** means the current element I think

```
@var: #004590;

div{
  height: 50px;
  width: 50px;
  background-color: @var;

  &:hover{
    background-color: fadeout(@var, 50%)
  }
}

```
