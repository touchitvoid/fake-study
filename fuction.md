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

