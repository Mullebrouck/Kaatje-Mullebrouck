# Loading-spinner

In this tutorial we are going to learn how to create a **"loading-spinner"** in HTML and CSS. 

Before we begin make sure you have a HTML document with a link to your CSS stylesheet. (Example: index.html & spinner.css)


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

Open your **spinner.css** file and add your `spinner` class. 

```css
.spinner {
}
```
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

Now we will make the border



