# Styled Components

[Styled Components Website](https://www.styled-components.com/)

There are many options for dealing with css styles in React. Styled Components is one. You basically are able to create
React Components that have styles applied to them:

First npm install it in your project:
```bash
npm install styled-components
```

Then use it in your components like this:
```js
import React from 'react'
import styled from 'styled-components'

// - note that styled is the package (object)
// - with styled.something, the something is the html div u want it to be under the hood
// - it uses backticks so you can write css in a string on different lines
// - if your css is all one color, it means your editor doesnt recognize styled components syntax, installing 
//   a syntax package on your code editor is worth it.
const Container = styled.div`
  height: 100px;
  width: 100px;
  border-radius: 5px;
  padding: 20px;
`

const Button = styled.button`
  padding: 20px 10px;
  background: #222;
  color: white;
  border: none;
  border-radius: 20px;
`

class Comp extends React.Component {
  render() {
  
    return <Container>
      <h1>Signup Form</h1>
      <Button>Click Here</Button>
    </Container>

  }
}

export default Comp


```


Also, if your component has no logic and is just styles, you can just return a function:
```js
import React from 'react'
import styled from 'styled-components'

const Container = styled.div`
  height: 100px;
  width: 100px;
  border-radius: 5px;
  padding: 20px;
`

const Button = styled.button`
  padding: 20px 10px;
  background: #222;
  color: white;
  border: none;
  border-radius: 20px;
`

export default () => {
  return <Container>
      <h1>Signup Form</h1>
      <Button>Click Here</Button>
    </Container>
}

```
