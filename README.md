# learnTips
工作中遇到的一些点

## ES6 
<code>import { jsonParse } from 'body-parser'</code>
<br>
效果等同于<br>
<code>var jsonParse = require('body-parser').jsonParse</code>
<br>


<code>
const { body, body: { username, password } } = request
</code>
<br>
效果等同于
<br>
<code>
  var body = request.body<br>
  var username = body.username<br>
  var password = body.password<br>
</code>
