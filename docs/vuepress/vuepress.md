## vuepress的使用

### 环境要求

nodejs

### 安装vuepress

```powershell
npm install -g vuepress
```

### 创建文件夹并进入

```powershell
mkdir nameblogs
cd nameblogs
```

### 初始化文件

```powershell
npm init -y
```

### 配置启动命令

修改package.json文件 内 scripts的内容

`  "dev": "vuepress dev docs --temp .temp",`意思是启动服务 并启用热加载

热加载：服务启动后改了改变内容网页自动变化，如果不启动热加载，文件内容改变网页还是不改变，需要重新启动服务才会加载更新的内容

`  "build": "vuepress build docs"`  意思是生成静态文件

```powershell
  "dev": "vuepress dev docs --temp .temp",
  "build": "vuepress build docs"
```

### 基本配置以完成 试着跑起来看看

```powershell
npm run dev
```



### 具体使用

1、改变启动端口

编辑docs/.vuepress/config.js

```js
// module.exports = {内配置}
module.exports = {
  port:80,
```


