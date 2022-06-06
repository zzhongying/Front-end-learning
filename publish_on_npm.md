## 将自己的包发布在npm上

### 1.在npm上创建一个账户 https://www.npmjs.com/
### 2.在项目终端使用npm init命名初始化想要发布的包，一路回车或者设置自己想要修改的内容就行
### 3.在项目终端上使用npm login登录之前创建好的账户，出现“Logged in as ‘自己的用户名’ on  https://registry.npmjs.org/” 即可
### 4. 使用npm publish发布自己的包，此时有几个注意事项
- 在package.json中，将private设置为fasle，表示不是私有包
- 初次publish可能会报错“ You do not have permission to publish "包的名称". Are you logged in as the correct user?”
- 这是因为当前发布的包和已存在的包重名了，所以需要自己去package.json中修改name属性
