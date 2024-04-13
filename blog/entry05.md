# Entry 5
##### 4/8/24

### How did you learn about your tool?
With SASS it opens a whole new world when writing code in your CSS. In this [basic tutorial from w3schools](https://www.w3schools.com/sass/) it explains how SASS is different from your normal CSS. As you can see from the SASS tutorial it helps reduce the amount of repetition. Normal you would do `background-color: color;` for CSS to change the background color of your website but with SASS you can do `bgcolor: color;` and this will do the same thing but more efficiently since you have to type less. Now its your turn](https://www.w3schools.com/sass/showsass.php?filename=demo_sass_first) by trying out that demo since the first step to learning something is by reading and then actually trying to do it yourself. 

### What you learned about your tool
I learned that With SASS you can have placeholders. These placeholders are useful for writing code that you dont want to repeat over and over. one example is:
```
%media
  overflow: hidden
  &:first-child
    float: left
  &:last-child
    overflow: hidden
```
This code allows for the media to become more flexable on where you want to put it.
Similar to the placeholders we also have `@extend`.
What @extend does is that it shares the properties of one CSS code with another one, for example, this code from w3schools:
```
.button-basic  {
  border: none;
  padding: 15px 30px;
  text-align: center;
  font-size: 16px;
  cursor: pointer;
}

.button-report  {
  @extend .button-basic;
  background-color: red;
}
```
The @extend here takes all the properties that are in ".button-basic" and shares them in ".button-report". By doing it saves you the time of having to copy and paste all of the previous code if you wanted to use it again. [Link to the w3school code](https://www.w3schools.com/sass/sass_extend.php) 
I learned what @mixin can do. What it does is it lets you create CSS code that is to be reused throughout the website. I also learned that @include was created to let you use the @mixin. One example of me tinker with this was:
```
@mixin border {
  margin: 5;
  padding: 5;
}

@mixin horizontal-list {
  @include border;

  li {
    display: inline-block;
    margin: {
      right: -8px;
      left: 5em;
    }
  }
}
```
This code uses @include to include the css from the border into where ever u place it. The @mixin is used as a class that can be reused. 



[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
