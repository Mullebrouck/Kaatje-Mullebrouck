# Transforming html into react.js


Example of how to transform HTML code into react.js

```html
<!DOCTYPE html>
<html>
  <div class='comment-box'>
    <h2>Comments</h2>
    <h4 class='comment-count'>4 comments</h4>
    <div class='comment-list'>
      <div class='comment'>
        <p class='comment-header'>Learning React.js</p>
        <p class='comment-body'>I have a question about learning react.js.</p>
        <div class='comment-footer'>
          <a href='#' class='delete-comment'>
            Delete Comment
          </a>
        </div>
      </div>
    </div>
  </div>
</html>
```

We can find two components in here: 
- comment-box
- comment


---


**Let's write first the 'comment' component**


```js
class Comment extends React.Component {
  render() {
    return (
      <div className='comment'>
        <p className='comment-header'>Learning React.js</p>
        <p className='comment-body'>I have a question about learning react.js.</p>
        <div className='comment-footer'>
          <a href='#' className='delete-comment'>
            Delete Comment
          </a>
        </div>
      </div>
    );
  }
}

```
- We changed all the html classes into className=' '
- if we want to use this component we can use it as ``<comment/>``

<br>
**Let's write now or 'comment-box' component** <br>

We are going to call or comment component in this one. 

```js
class CommentBox extends React.Component {
  render() {
    return (
      <div className='comment-box'>
        <h2>Comments</h2>
        <h4 className='comment-count'>4 comments</h4>
        <div className='comment-list'>
          <comment author="" body=""/>
          <comment author="" body=""/>
          <comment author="" body=""/>
          <comment author="" body=""/>
        </div>
      </div>
    );
  }
}
```

The problem here is that all the comments will look the same, so we have to add arguments (called props in React).

```js
class Comment extends React.Component {
  render() {
    return (
      <div className='comment'>
        <p className='comment-header'>{this.props.author}</p>
        <p className='comment-body'>{this.props.body}</p>
        <div className='comment-footer'>
          <a href='#' className='delete-comment'>
            Delete Comment
          </a>
        </div>
      </div>
    );
  }
}
