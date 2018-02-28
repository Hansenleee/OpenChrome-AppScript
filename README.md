# OpenChrome-AppScript
通过AppScript判断打开指定URL

目前只支持mac下的谷歌浏览器

## 使用方式
```
osascript open "https://www.baidu.com"
```
传入URL地址

## 应用场景
可配合前端node项目搭建好自动打开项目地址
例如：
```javascript
  createHttpServer().then(() => {
    var url = 'http://localhost:8080'
    const execSync = require('child_process').execSync
    execSync('osascript open-url "' + url + '"', {
      cwd: __dirname,
      stdio: 'ignore',
    });
  })
```

## 记录一个AppleScript学习地址
[AppleScipt 文档](http://vdisk.weibo.com/s/CPqex2XUrgEq)
