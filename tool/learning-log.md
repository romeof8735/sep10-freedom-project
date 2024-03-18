# Tool Learning Log

Tool: **SASS**

---

2/28/24:
* [SASS](https://sass-lang.com/)
* With SASS it opens a whole new world when writing code in your CSS
* In this [basic tutorial from w3schools](https://www.w3schools.com/sass/) it explains how SASS is different from your normal CSS
* As you can see from the SASS tutorial it helps reduce the amount of repetition
* Normal you would do `background-color: color;` for CSS to change the background color of your website but with SASS you can do `bgcolor: color;` and this will do the same thing but more efficiently since you have to type less
* [Now its your turn](https://www.w3schools.com/sass/showsass.php?filename=demo_sass_first) by trying out that demo since the first step to learning something is by reading and then actually trying to do it yourself

3/1/24:
* I would recommend watching [this video](https://www.youtube.com/watch?v=akDIJa0AP5c) that sums up what SASS is in under 3 minutes
* The person who explains this video talks a bit fast but what he is basically explaining is that SASS has 3 important features that CSS doesnt have which is "Nesting" "Mixins" and "Functions"
* One thing that I thought was pretty cool is that if you remember anything that we did in code.org when we were in 9th grade was that we would use things such as if or else and in SASS functions they also use that same if or else
* If you want to watch a bit longer video of someone explaining these things in detail I would recommend watching this [20 minute video](https://www.youtube.com/watch?v=Zz6eOVaaelI)


3/10/24:
* With SASS you can have placeholders.
* These placeholders are useful for writing code that you dont want to repeat over and over
* one example is:
```
%media
  overflow: hidden
  &:first-child
    float: left
  &:last-child
    overflow: hidden
```
* This code allows for the media to become more flexable on where you want to put it

3/18/24:
* Similar to the placeholders we also have `@extend`
* What @extend does is that it shares the properties of one CSS code with another one, for example:
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
* The @extend here takes all the properties that are in ".button-basic" and shares them in ".button-report"
* By doing it saves you the time of having to copy and paste all of the previous code if you wanted to use it again

<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
