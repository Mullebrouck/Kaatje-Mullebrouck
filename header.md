## Header Text Image Replacement

- If customer wants a font that is not supported
- No assistive technology, but other way: 

    - Code company website with `<h1>` element
    - Configure styles for header element: set header banner image as background of header or `<h1>` element
    - Use `text-indent` property to configure placement of `<h1>` text outside of the browser viewport (Most Commonly Used: `text-indent: -9999px;`


- sometimes issue on mobile devices, fix with: 

 ```css
 h1 {
    text-indent: 100%; /*Instead of -9999*/
    white-space: nowrap;
    overflow: hidden;
 }
 ```
 Example: 
 
 ```CSS
 
 header {
    height: 150px;
    margin-bottom: 10px;
    background-image: url(banner.jpg);
    background-repeat: no-repeat;
 } 
 
  h1 {
    text-indent: 100%; /*Instead of -9999*/
    white-space: nowrap;
    overflow: hidden;
 }
 
 ```