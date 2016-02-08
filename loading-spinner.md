# Loading-spinner

In this tutorial we are going to learn how to create a **"loading-spinner"** in HTML and CSS. 

Before we begin make sure you have a HTML document with a link to your CSS stylesheet. (Example: index.html & spinner.css)



---


We will start by adding a `<div>` element in your HTML `<body>` element. We will add a `class` called **loading-spinner** within the `<div>`.


<br>
**Index.html**
```html
<!DOCKTYPE html>
    <head>
        <meta charset="utf-8">
        <title>Loading-Spinner</title>
        <link rel="stylesheet" href="spinner.css">
    </head>
    <body>
        <div class="loading-spinner"> </div>
    </body>
</html>

```


---


Open your **spinner.css** file and add your `loading-spinner` class. 

```css
.loading-spinner {
}
```


---


We will now add a `height` and  a `width` into your class, that will define how big your **loading-spinner** will be. Add also a `border`, that we will use to make the spinner. 

```css
.loading-spinner {
    height: 50px;
    width: 50px;
    border: 5px solid #FFB43B;
}
```
It should look like this:

![](Screen Shot 2016-02-07 at 7.46.19 PM.png)


---


Now we want to change the border into a **circular shape**. We can do this by adding `border-radius`.

- 50% - 100% will make your border round. 

```css
.loading-spinner {
    height: 50px;
    width: 50px;
    border: 5px solid #FFB43B;
    border-radius: 100%;
}
```

Now we have a circular border:

![](Screen Shot 2016-02-07 at 8.15.38 PM.png)


---

We are going to change our `border-color`, so when it spins you will see a **gradient effect**. 

- leave the original color at the `top`
- create slightly lighter color for the `left`
- create lighter color for the `bottom`
- make `right`color `tranpsarent`


```css
.loading-spinner {
    height: 50px;
    width: 50px;
    border: 5px solid #FFB43B;
    border-radius: 100%;
    border-left-color:#F6C068;
    border-bottom-color: #F3D19A;
    border-right-color: transparent;
}
```

This is how it should look like:

![](Screen Shot 2016-02-07 at 8.25.26 PM.png)


---
In this step we will apply the **animation** by using the `@` rule with `keyframes`. We want to make sure we give our animation a name, lets call it **spinner.** 


```css
.loading-spinner {
    height: 50px;
    width: 50px;
    border: 5px solid #FFB43B;
    border-radius: 100%;
    border-left-color:#F6C068;
    border-bottom-color: #F3D19A;
    border-right-color: transparent;
}

@keyframes spinner {

}
```

In some cases you have to install a **CSS pre-fix**. You can check the website http://caniuse.com/ to see with browser support these pre-fixes and for which browsers you still need to **implement** them.  In this case, all the browsers support the `@keyframes` rule. 

---

We want our `loading-spinner` to spin from 0-100% so we will have to add a **360 degrees rotation** in our animation. 

```css 
@keyframes spinner {
    100% {
        transform: rotate(360deg);
    }
}
```


---

Now we want to implement this **animation** into our `loading-spinner` class, we do this by adding the `animation` property. We also need to add the **name of the animation**, the **time** the animation needs to complete, how many times the animation will **repeat** and a **type**. 

```css
.loading-spinner {
    height: 50px;
    width: 50px;
    border: 5px solid #FFB43B;
    border-radius: 100%;
    border-left-color:#F6C068;
    border-bottom-color: #F3D19A;
    border-right-color: transparent;
    animation: spinner 0.5s infinite linear;
}

@keyframes spinner {
    100% {
        transform: rotate(360deg);
    }
}
```

Now our animation is complete. To see an **example** of this **loading-spinner** you can look at my codepen: http://codepen.io/Kaatje/pen/Bjqggd?editors=1100

---
