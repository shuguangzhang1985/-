# learnTips
工作中遇到的一些点

## ES6 
<code>import { jsonParse } from 'body-parser'</code>
效果等同于
<code>var jsonParse = require('body-parser').jsonParse</code>

<code>
const { body, body: { username, password } } = request
</code>
效果等同于
<code>
  var body = request.body
  var username = body.username
  var password = body.password
  </code>
