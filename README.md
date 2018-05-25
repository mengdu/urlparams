# urlparams

url 参数设置

```js
const urlparams = require('./dest').default

let url = 'http://www.baidu.com'
let newUrl = urlparams.url(url, {
  name: 'test',
  order: 'desc',
  zh: '中文',
  in: ['test', 'demo', 'debug'],
  obj: {
    attr: 12
  },
  json: JSON.stringify({title: 'http://www.baidu.com?xx=张三'})
}, true)

console.log(newUrl)
```

# API

urlparams.url(url, params, isEncode) 为url添加参数
