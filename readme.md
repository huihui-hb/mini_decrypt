## 微信小程序反编译

这个操作好像没有什么用，我逆向一些其他人的接口。

### 从电脑上打开微信小程序保存位置。 

可以从微信的设置中进入微信文件夹 再Applet\{wxid} ，app.wxpkg就是主包

### 使用解密

具体原理参考老哥的原理文档，这边有人家写的最终程序

```
pc_wxapkg_decrypt.exe -wxid 微信小程序id -in 要解密的wxapkg路径 
```

### 反编译

先安装依赖,npm i （需要node环境），再在本目录下运行
```
node .\wuWxapkg.js .\dec.wxapkg
```

