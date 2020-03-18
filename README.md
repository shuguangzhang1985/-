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
  var body = request.body
  
  var username = body.username
  
  var password = body.password
</code>

## export import
1.当用export default people导出时，就用 import people 导入（不带大括号）

2.一个文件里，有且只能有一个export default。但可以有多个export。

3.当用export name 时，就用import { name }导入（记得带上大括号）

4.当一个文件里，既有一个export default people, 又有多个export name 或者 export age时，导入就用 import people, { name, age } 

5.当一个文件里出现n多个 export 导出很多模块，导入时除了一个一个导入，也可以用import * as example

## git 指令
命令行指令

Git 全局设置
```git config --global user.name "张曙光"
git config --global user.email ""
```

创建新版本库
git clone git@code.aliyun.com:vue-group/jd-merchant.git
cd jd-merchant
touch README.md
git add README.md
git commit -m "add README"
git push -u origin master

已存在的文件夹或 Git 仓库
cd existing_folder
git init
git remote add origin git@code.aliyun.com:vue-group/jd-merchant.git
git add .
git commit
git push -u origin master

