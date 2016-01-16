# HTML Email

#Email.html

Use Inline styles!

```html
<!DOCTYPE html>
<html> 
  <head>
    <meta charset="utf-8">
    <title>HTML Email Base</title>
    <meta name="viewport" content="width=device-width" />
  </head>

  <body style="margin:0; padding:o;"> <!-- resetting styles-->

    <!--adding background to complete -->
    <div style=" 
        background-color: ...;
        background-image: url(...png); ">

      <!--to make everything the same width add a <div> -->
      <div style="
          margin: 0 auto; <!-- reset style -->
          max-width: 600px;
          text-align: center; <!-- to clean it up a little --> ">

        <!-- When adding image to html you need to use absolute url -->
        <img src="http://...png" style=" 
           background-color: ...;
           display: ...;
           max-width: 100%
           padding: 12px o;"
           width="..."; /> <!-- no need to add px, because it will read it in px-->

        <!--adding styles to each < > -->
        <h1 style="
           color: ...;
           font-family: .....;
           font-size: ....;
           line-height: ....;
           margin: 0; <!-- reset styles -->
           text-transform: ...; ">
           ...</h1>

        <!-- using container, font and reset styles -->
        <p style="
           background: ...; 
           color: ...; 
           font-family: .....; 
           font-size: ....; 
           line-height: ....; 
           margin: 0; 
           padding: ...; 
           text-transform: ...; "> 
           ...
           </p>     
      </div>
    </div>
  </body>
</html>
```



 