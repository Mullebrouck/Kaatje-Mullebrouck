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

In this step we will add a `border` that helps to create the shape of the spinner. We will need to add  a `height` and  a `width` into the class. This will define how big your **loading-spinner** will be.

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

Now we have a circular shape:

![](Screen Shot 2016-02-07 at 8.15.38 PM.png)


---

We are going to change our `border-color`, so when the spinner spins you will see a **gradient trail**. 

- leave the original color at the `border-top`
- create slightly lighter color for the `border-left`
- create lighter color for the `border-bottom`
- make `border-right`color `tranpsarent`


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
@keyframes spinner {

}
```

In some cases you have to install a **CSS pre-fix**. You can check the website http://caniuse.com/ to see which browser supports these CSS features, and which need pre-fixes to run in experimental mode because they don't officially support the feature yet. In this case, all the browsers support the `@keyframes` rule.  

---

We want our `loading-spinner` to spin from "0" being the start of the animation to 100% what indicates the end of the animation. We also want to add a **360 degrees rotation** in our animation. 

```css 
@keyframes spinner {
    100% {
        transform: rotate(360deg);
    }
}
```


---

Now we want to implement this **animation** into our `loading-spinner` class, we do this by adding the `animation` property. We also need to add the **name of the animation**, the **time** the animation needs to complete one loop or circle, how many times the animation will **repeat** and the acceleration **type**. For this example we choose a **linear** type, so the speed thoughout the animation won't change. 


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
Now we want to add this animation to our webpage. 
In this tutorial, we will add and display the **loading-spinner** when we click the **submit button** in our form. In this form the user will have to enter his/her email address.

Lets take a look at our `form`:

![](Screen Shot 2016-02-07 at 10.19.53 PM.png)

When the user **clicks** on the submit button, the **loader-spinner** will shown until the submitting is complete and the page refreshes. 

**HTML File**

```html
<form class="subscription">
  <label>Subscribe</label>
  <input class="text" type="email" placeholder="Enter email address">
  <input class="button" type="submit" value="Click to submit">
</form>
```

**CSS File**

```css
.subscription {
  background-color: #6D6963;
  border-radius: 5%;
  height:200px;
  text-align: center;
  width: 300px;
}

label {
  color: #FCF8F1;
  display: block;
  font-family: Avenir;
  font-weight: bold;
  font-size: 30px;
  padding-top: 30px;
}

.text {
  border-radius: 5%;
  height: 20px;
  margin: 20px;
  text-align: center;
  width: 200px;
}

.button {
  background-color: #FFB43B;
  border-radius: 5%;
  color: #6D6963;
  display: block;
  font-family: Avenir;
  font-weight: bold;
  font-size: 10x;
  height: 25px;
  margin: 0 auto;
  width: 120px;
}
```


---

Now we will add our **loading-spinner** into our **HTML** and **CSS** file.

**HTML File**
```HTML
<form class="subscription">
  <label>Subscribe</label>
  <input class="text" type="email" placeholder="Enter email address">
  <input class="button" type="submit" value="Click to submit">
</form>

<div class="loading-spinner"> </div>
```
**CSS File**
```css
.loading-spinner {
    animation: spinner 0.5s infinite linear;
    border: 5px solid #FFB43B;
    border-radius: 100%;
    border-left-color:#F6C068;
    border-bottom-color: #F3D19A;
    border-right-color: transparent;
    height: 15px;
    width: 15px;
}

@keyframes spinner {
    100% {
        transform: rotate(360deg);
    }
}

.subscription {
  background-color: #6D6963;
  border-radius: 5%;
  height:200px;
  text-align: center;
  width: 300px;
}

label {
  color: #FCF8F1;
  display: block;
  font-family: Avenir;
  font-weight: bold;
  font-size: 30px;
  padding-top: 30px;
}

.text {
  border-radius: 5%;
  height: 20px;
  margin: 20px;
  text-align: center;
  width: 200px;
}

.button {
  background-color: #FFB43B;
  border-radius: 5%;
  color: #6D6963;
  display: block;
  font-family: Avenir;
  font-weight: bold;
  font-size: 10x;
  height: 25px;
  margin: 0 auto;
  width: 120px;
}
```

What should result like this:

![](Screen Shot 2016-02-07 at 10.16.31 PM.png)


---

We can see in our example image that our **loading-spinner** is now displayed **underneath** the form. We want to add the `.loading-spinner` div inside our `form`. 

**HTML File**
```HTML
<form class="subscription">
  <div class="loading-spinner"> </div>
  <label>Subscribe</label>
  <input class="text" type="email" placeholder="Enter email address">
  <input class="button" type="submit" value="Click to submit">
</form>
```


You can now see that the `.loading-spinner` is now displayed in the upper left corner. 

![](Screen Shot 2016-02-07 at 10.16.48 PM.png)


---



Now we will add some styles in our CSS so we can center our `.loading-spinner` in the middle of our form. We also want to add a `position: absolute` so we can move the `class` without pushing it's siblings. 

```CSS
.loading-spinner {
    left: 150px;
    position: absolute;
    top: 100px;
    
    animation: spinner 0.5s infinite linear;
    border: 5px solid #FFB43B;
    border-radius: 100%;
    border-left-color:#F6C068;
    border-bottom-color: #F3D19A;
    border-right-color: transparent;
    height: 15px;
    width: 15px;
}
```

Your form should look similar like this: 

![](Screen Shot 2016-02-07 at 11.01.50 PM.png)


---

We only want to see our **loading-spinner** when the form is being submitted, so we will have to add a few lines of **JavaScript**. But first lets add `diplay:none;` to our `.loading-spinner`class styles.

```CSS
.loading-spinner {
    display: none;
    left: 150px;
    position: absolute;
    top: 100px;
    
    animation: spinner 0.5s infinite linear;
    border: 5px solid #FFB43B;
    border-radius: 100%;
    border-left-color:#F6C068;
    border-bottom-color: #F3D19A;
    border-right-color: transparent;
    height: 15px;
    width: 15px;
}
```

Now our **loading-spinner** is not displayed anymore. 

![](Screen Shot 2016-02-07 at 11.06.12 PM.png)


---

There are **two ways** to add our **JavaScript** file into our HTML. 
- We can use a `<script> </script>` tag in our `<head>`:  

```html
<!DOCKTYPE html>
    <head>
        <meta charset="utf-8">
        <title>Loading-Spinner</title>
        <link rel="stylesheet" href="spinner.css">
        <script>
            Add here your JavaScript
        </script>
    </head>
    <body>
        <div class="loading-spinner"> </div>
    </body>
</html>

```

- or we can add a `.js` file, dont forget to add the `</script>` closing tag:

```html
<!DOCKTYPE html>
    <head>
        <meta charset="utf-8">
        <title>Loading-Spinner</title>
        <link rel="stylesheet" href="spinner.css">
        <script src="file.js"> </script>
    </head>
    <body>
        <div class="loading-spinner"> </div>
    </body>
</html>

```


---
Now we are ready to write our **JavaScript**. 

- In our first line we want to **create a variable** that will point to the **submit button**. 
- In our second line we want to **create a variable** that will point to the **form**.
- Now we want to **create** a new class `loading`. We will set the button to **add** this class `loading` to the form when the button is clicked. When you add the `loading` class, the CSS will display the `**loading-spinner** untill submitting is complete & will refresh the page.


JavaScript: 

```js
var submitbutton = document.querySelector('.button');
var form = document.querySelector('.subscription');
submitbutton.onclick = function (){
  form.classList.add('loading')
}
```


---

To make sure our **loading-spinner** displays we need to add the new class `loading` into our CSS file: 

```CSS
.loading .loading-spinner {
  display: block;
}
```


---



Now our **loading-spinner** is **ready to display** once the submit button is clicked. 



To see an **example** of this you can surf to the following link and check out my codepen. 
http://codepen.io/Kaatje/pen/Bjqggd

---



---



