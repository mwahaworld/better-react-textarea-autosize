# better-react-textarea-autosize
Fork of [https://github.com/andreypopp/react-textarea-autosize](react-textarea-autosize). Includes everything from the original package, but allows to create a ref to component.

## Install
```
npm install better-react-textarea-autosize
```

## ref usage
```js
import React, { Component } from 'react';
import Textarea from 'better-react-textarea-autosize';

class MyTextarea extends Component {
  componentDidMount() {
    this.field.focus();
  }

  render() {
    return (
      <Textarea
        inputRef={(node) => { this.field = node; }}
      />
    );
  }
}
```

## Demo
https://andreypopp.github.io/react-textarea-autosize/
