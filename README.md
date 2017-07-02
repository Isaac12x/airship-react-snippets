# Airship React Snippets

This is a collection of React Snippets to make your fingers a little happier.

## Installation

In order to install an extension you need to launch the Command Pallete (Ctrl + Shift + P or Cmd + Shift + P) and type Extensions.
There you have either the option to show the already installed snippets or install new ones.

Launch VS Code Quick Open (Ctrl + P or Cmd + P), paste the following command, and press enter.

`ext install airship-react-snippets`

Alternatively you can open the extensions panel and search for 'Airship React Snippets'.

## Supported languages (file extensions)

* Javascript (.js)

## Snippets

__imp__
```
import $1 from '$2';
```

__impr__
```
import React from 'react';
```

__imprc__
```
import React, { Component } from 'react';
```

__imprn__
```
import { $1 } from 'react-native';
```

__imprr__
```
import { connect } from 'react-redux';
```

__impaa__
```
import * as $1 from '$2';
```

__afn__
```
$1 = ($2) => {
  $3
};
```

__eafn__
```
export default ($1) => {
  $2
};
```

__enfn__
```
export const $1 = ($2) => {
  $3
};
```

__prom__
```
return new Promise((resolve, reject) => {
  $1
});
```

__rinit__
```
import React from 'react';
import ReactDOM from 'react-dom';

ReactDOM.render(
  $2
  , document.querySelector('$1')
);
```

__rcc__
```
class $1 extends Component {
  state = { $2 };

  render() {
    return (
      $3
    );
  }
}

export default $1;
```

__recc__
```
export default class $1 extends Component {
  state = { $2 };

  render() {
    return (
      $3
    );
  }
}
```

__ris__
```
this.state = {
  $1
};

```

__rss__
```
this.setState({
  $1: $2
});
```

__rs__
```
this.state.$1
```

__rcpt__
```
$1.propTypes = {
  $2
};

$1.defaultProps = {

};
```

__rp__
```
this.props.$1
```

__rcon__
```
constructor(props) {
  $1
}
```

__rren__
```
render() {
  return (
    $1
  );
}
```

__rcwm__
```
componentWillMount() {
  $1
}
```

__rcdm__
```
componentDidMount() {
  $1
}
```

__rcwum__
```
componentWillUnmount() {
  $1
}
```

__rcwu__
```
componentWillUpdate(nextProps) {
  $1
}
```

__rcdu__
```
componentDidUpdate(prevProps, prevState) {
  $1
}
```

__rcwrp__
```
componentWillReceiveProps(nextProps) {
  $1
}
```

__rsc__
```
const $1 = () => (
  $2
)

export default $1;
```

__rhoc__
```
import React, { Component } from 'react';

export default function(ComposedComponent) {
  class $1 extends Component {
    render() {
      return <ComposedComponent {...this.props} />;
    }
  }

  export default $1;
}
```

__rrinit__
```
import React from 'react';
import ReactDOM from 'react-dom';
import { Provider } from 'react-redux';
import { createStore, applyMiddleware } from 'redux';

import reducers from './reducers';

const createStoreWithMiddleware = applyMiddleware()(createStore);

ReactDOM.render(
  <Provider store={createStoreWithMiddleware(reducers)}>
    $2
  </Provider>
  , document.querySelector('$1')
);
```

__rrcr__
```
import { combineReducers } from 'redux';
import $1 from './$2';

const rootReducer = combineReducers({
  $3
});

export default rootReducer;
```

__rccc__
```
import React, { Component } from 'react';
import { connect } from 'react-redux';

class $1 extends Component {
  render() {
    return (
      $2
    );
  }
}

const mapStateToProps = (state) => ({
  $3
});

export default connect(mapStateToProps)($1);
```

__rred__
```
export default (state = $1, action) => {
  switch(action.type) {
    case $2:
      $3
    default:
      return state;
  }
}
```

__rmstp__
```
const mapStateToProps = (state) => ({
  $1
});
```

## License

MIT License

Copyright (c) 2017 Airship, LLC

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

