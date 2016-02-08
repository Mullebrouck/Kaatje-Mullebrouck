# Loading-spinner

In this tutorial we are going to learn how to create a **"loading-spinner"** in HTML and CSS. 

Before we begin make sure you have a HTML document with a link to your CSS stylesheet. (Example: index.html & spinner.css)



---


We will start by adding a `<div>` element in your HTML `<body>` element. We will add a `class` called **spinner** within the `<div>`.


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
        <div class="spinner"> </div>
    </body>
</html>

```


---


Open your **spinner.css** file and add your `spinner` class. 

```css
.spinner {
}
```


---


We will now add a `height` and  a `width` into your class, that will define how big your **loading-spinner** will be. Add also a `border`, that we will use to make the spinner. 

```css
.spinner {
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
.spinner {
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
.spinner {
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
In this step we will apply the **animation** by using the `@` rule with `keyframes`. We want to make sure we give our animation a name, lets call it **spin.** 


```css
.spinner {
    height: 50px;
    width: 50px;
    border: 5px solid #FFB43B;
    border-radius: 100%;
    border-left-color:#F6C068;
    border-bottom-color: #F3D19A;
    border-right-color: transparent;
}

@keyframes spin {

}
```

In some cases you have to install a **CSS pre-fix**. You can check the website http://caniuse.com/ to see with browser support these pre-fixes and for which browsers you still need to **implement** them.  In this case, all the browsers support the `@keyframes` rule. 


---


