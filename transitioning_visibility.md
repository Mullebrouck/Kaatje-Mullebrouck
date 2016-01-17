# Transitioning Visibility


### Creating Form and Overlay

```html
<div class='modal-overlay'></div>

<div class='modal'>
    <div class='modal-header'>
        <a class='modal-close'>&times;</a>
        <h3>Your header title</h3>
    </div>

    <div class='modal-content'>
        <form class='form' action=''>
         ...
        </form>
    </div>
</div>
```
Initial Modal State: Hidden

```css
.modal,
.modal-overlay {
    visibility: hidden;
    Opacity: 0;
}

/*active class is added when you click the button*/
.modal.active,
.modal-overlay.active {
    opacity: 1;
    visibility:visible;
}
```

>Not al properties can be transitioned in css, so do not use display: none;  it will remove your element. 

Opacity: 0;  —> Hides element, but element still takes up same width and height +
Visibility: hidden; (Makes element transparent to click events)

```css
.modal,
.modal-overlay {
    /*Visibility: hidden; (Makes element transparent to click events)*/
    visibility: hidden;
    /* Opacity: 0;  —> Hides element, but element still takes up same width and height */
    Opacity: 0; 
    transition: opacity .5s, visibility .5s;
    /* or you can use */
    transition: all .5s;
}
```
