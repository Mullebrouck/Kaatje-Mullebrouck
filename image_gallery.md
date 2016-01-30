# Image Gallery with Unordered List

**Example Image Gallery**

```HTML
<ul>
    <li>
        <img src="photo1.jpg" alt="picture1" width="225" height="168">
    </li>
    <li>
        <img src="photo2.jpg" alt="picture2" width="225" height="168">
    </li>
    <li>
        <img src="photo3.jpg" alt="picture3" width="225" height="168">
    </li>
</ul>
```

```CSS
ul {
    list-style-type: none;
}

li {
    display: inline-block;
    width: 225px;
    padding-bottom: 10px;
    margin: 10px;
    background-color: #EAEAEA;
    text-align: center;
    font-style: italic; 
    font-family: Georgia, serif;
}
```

