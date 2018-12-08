# Part 2, Basic HTML/CSS/JS (Windows Instructions)

* Delete the `<p>` tag and write this instead

```
<main>
    <section class="hero">
        <div class="col-1 row-2"></div>
        <h1 class="col-2 row-2">Welcome! to the<br>new world order</h1>
        <div class="col-3 row-2"></div>
    </section>
</main>
```
* Go into the `sass/style.scss` file and type the following

```
@import url('https://fonts.googleapis.com/css?family=Source+Sans+Pro');
*{
    margin: 0;
    //border:1px solid red;
}
body{
    font-family: 'Source Sans Pro', sans-serif;
}
div{
    height: 50px;;
}
```

* You should see some red outlines, this is the box-model and using the `* border:red` is super usefull. Now Write this content below the `</section>` tag. 

```
<div class="container">
    <div class="col-1 intro-text">
        <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p> 
    </div>
    <div class="col-2 intro-heading">
        <h2>
            How to take over the world!
        </h2>
        <a target="_blank" href="http://producthunt.com">See All The Products</a>
    </div>
</div>  
```
* Go back to your `style.scss` delete the `div { height }...` part and write this below the `body {}` declaration.

```
.container{
    display: grid;
    grid-template-columns: 1fr 1fr;
    max-width: 960px;
    margin:auto;
}
```

This should look like the following
![box model 1](images/box-model-1.png)