# React 


- Set up your HTML document
- In the body section you just write 
`<div class="container"></div>` --> this is where React will be injected. 


### Template for React


```javascript
// This gets the HTML element with class container
var container = document.querySelector('.container');

//Creates React element  
function Component ( ) {
  return (
    <div>  
      <h2 className='title'>A</h2>  
    </div>
  );
}

// Tells the browser to inject the 
// React element into the container tag (var container)
ReactDOM.render(<Component  />, container); 
```

