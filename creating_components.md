# Creating Components


**components.js**
```js
class StoryBox extends React.Component {
  render() {
    return (
      <div> Story Box </div>
      );
  }
}

ReactDOM.render(
  < StoryBox /> , document.getElementById("story-app") 
);

```
``StoryBox`` --> components are written in upper Camel Case <br>
``React.Components`` --> Inherits from the React Base class<br>
``render ()`` --> Every component will need a ``render()`` function<br>
``<div>`` --> html elements will always be in lowercase + No quotes are needed. <br>
``< StoryBox /> `` --> invokes the class StoryBox <br>
``getElementById`` --> Target container where component will be rendered to. <br>


