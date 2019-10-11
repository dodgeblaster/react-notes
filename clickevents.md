# Events in React

```js
import React from 'react'

class Comp extends React.Component {

  state = {
    launched: false
  }
  
  launch = () => {
    console.log('LAUNCH')
    this.setState({launched: true)
  }
  
  render() {
    return <div>
      <div
        style={{
          height: '100px',
          width: '100px',
          background: this.state.launched ? 'green' : 'grey'
        }}
      ></div>
      <button onClick={this.launch}>Launch</button>
    </div>
  }

}

export default Comp


```
