<img src="https://raw.githubusercontent.com/css-modules/logos/master/css-modules-logo.png" width="150" height="150" />

# 伪类选择器

因为 css 模块通过向元素添加类来工作，所以可以很容易地添加伪类选择器。

```css
/* component/text.css */
.text {
  color: #777;
  font-weight: 24px;
}
.text:hover {
  color: #f60;
}
```
``` js
/* component/text.js */
import styles from './text.css';

import React, { Component } from 'react';

export default class Text extends Component {

  render() {
    return (
      <p className={ styles.text }>Text with hover</p>
    );
  }

};
```
