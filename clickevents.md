#Events in React


```js

class Compp extends React.Component {
  
  launch = () => {
    console.log('LAUNCH')
  }
  
  render() {
    return <div>
      <button onClick={this.launch}>Launch</button>
    
    </div>
  }

}


```
