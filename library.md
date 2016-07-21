# Library

- when writing custom methods we use a underscore to distinguish them.


### Display Current Time

**components.js**

```js
class StoryBox extends React.Component {
  render () {
    const now = new Date();
   
    return 
      <div>
        <h2> Title </h2>
        <p className = "paragraph">
          Current Time: { now.toTimeString() };
        </p>
      </div>
  }
}
```
**Outcome:** Current Time: shows exact time 

### Display List

**components.js**

```js
class StoryBox extends React.Component {
  render () {
    const list = ['one', 'two', 'four'];
   
    return 
      <div>
        <h2> Title </h2>
        <ul>
          {list.map(topic => <li>{topic}</li>)}
        <ul>
      </div>
  }
}
```
**Outcome:** 
- one
- two
- four



