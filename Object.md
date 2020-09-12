---


---

<p>const key = ‘test Key’<br>
const obj = {<br>
[key]: ‘this is key’<br>
}<br>
// 动态键名<br>
obj[‘test Key’] // this is key</p>
<p>let a =  {}<br>
let b = a</p>
<p>a === b // true<br>
let a,b = [{},{}]</p>
<p>let user =  { name:  “John”, sizes:  { height:  182, width:  50  }  };<br>
let clone = Object.assign({}, user);<br>
alert( user.sizes === clone.sizes );  // true，<br>
对象里的第二层对象依然是引用关系</p>

