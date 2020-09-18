---


---

<p><strong>函数也是一个对象</strong></p>
<h5 id="利用这一点有了以下记忆函数的用法-给函数添加了一个属性roles-函数存在则该roles存在">利用这一点有了以下记忆函数的用法 给函数添加了一个属性roles 函数存在则该roles存在</h5>
<pre><code>function isPrimary(value) {
    // create cache
    if (!isPrimary.roles) isPrimary.roles = {}
    // cache find
    if (isPrimary.roles[value]) return isPrimary.roles[value]
    // insert role to cache
    isPrimary.roles[value] = value
}
isPrimary('feizao')
console.log(isPrimary.roles) // { feizao: 'feizao' }
</code></pre>
<p><strong>IIFE自执行函数</strong><br>
弥补scope上的不足<br>
(fuction() {})()</p>
<p>arguments 类数组结构</p>
<p><strong>方法和函数</strong><br>
play() // 作为函数被调用<br>
feizao.play() //作为方法被调用</p>
<p>this指向调用函数的对象</p>
<p>构造函数返回一个对象则由该构造函数创建的实例对象为返回的对象</p>
<pre><code>const obj0 = { name: 'feizao' }
function _constructor () {
	this.name = 1
	return obj2
}
const obj1 = new _constructor()
console.log(obj1) // obj0
</code></pre>

