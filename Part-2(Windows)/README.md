# Part 2, Basic HTML/CSS/JS (Windows Instructions)

* Delete the `<p>` tag and write this instead
  
`index.html`
```
<main>
    <div>box #1</div>
</main>
```
`sass/style.scss`
```
main{
    color:red;
    border:1px solid red;
}
```
Your website should look like below
![box-model-image-1](images/box-model-1.png)

* Next we are going to add another `<div>` inside the `<main>` wrapper like so.

```
<main>
    <div>box #1</div>
    <div>box #2</div>
</main>
```
* Next add the following css, and your new styles should look like below

```
main{
    color:red;
    border:1px solid red;
}
div{
    border:1px solid aqua;
    margin: 10px;
}
```
Now your page should look something like this

![box-model-image-2](images/box-model-2.png)

* Now you are going to put these divs on the same line and then center the containing red `<main>` container, using some css declarations. First lets put those `<div>`'s on the same line
```
main{
    color:red;
    border:1px solid red;
    position:relative;
    float: left;
}
div{
    border:1px solid aqua;
    margin: 10px;
    float: left;
}
```
So here we added `float:left`'s and a `position:relative` this is the css box model, your page should look like below now

![box-model-image-3](images/box-model-3.png)

* Now we can't center the `<main>` element easily without stuff breaking, so we are going to add another `<div>` below center so you can see how we center stuff, and then we are going to refacor this code to use `display:flex` and then later `display:grid` currently the default is `display:block;` so let's add in another `<div>` At first you will see it stacks it next to the other div's, that is because we are giving every div a `float:left` lets change that, change your html to this

```

