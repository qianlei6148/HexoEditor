## 创建
### 总结 
```c
//Windows 配置npm使用:
npm config set prefix "C:/Program Files/nodejs/npm_global"
npm config set cache "C:/Program Files/nodejs/npm_cache" 

//Linux\Mac 配置npm使用:
npm config set prefix "~/nodejs/npm_global"
npm config set cache "~/nodejs/npm_cache" 

//如果在中国大陆，你可以设置镜像来加速!
npm config set registry "https://registry.npm.taobao.org"
npm config set electron_mirror "https://npm.taobao.org/mirrors/electron/"

git clone https://github.com/zhuzhuyule/HexoEditor.git
cd HexoEditor
npm install
npm start
```

### 操作详情
#### 1.安装 `git`
- [Mac OS X 下载](https://git-scm.com/download/mac) 
- [Windows 下载](https://git-scm.com/download/win) 
- [Linux/Unix 下载](https://git-scm.com/download/linux)

#### 2.安装 `nodejs`
- [下载地址](https://nodejs.org/en/download/) (英文)
- [下载地址](https://nodejs.org/zh-cn/download/) (中文)

**提示**

```c
//Linux/Uinx 设置连接方法
sudo ln -fs .../.../node-vX.X.X-linux-xXX/bin/node /usr/local/bin/node
sudo ln -fs .../.../node-vX.X.X-linux-xXX/bin/npm /usr/local/bin/npm

//或 如果无效
sudo ln -fs .../.../node-vX.X.X-linux-xXX/bin/node /usr/sbin/node
sudo ln -fs .../.../node-vX.X.X-linux-xXX/bin/npm /usr/sbin/npm
```
你可以使用命令 `which node` 来找到.

#### 3.配置

```c
//如果你想修改缓存地址
npm config set prefix "path of npm_global"
npm config set cache "path of npm_cache" 

//如果在中国大陆，你可以设置镜像来加速!
npm config set registry "https://registry.npm.taobao.org/"
npm config set electron_mirror "https://npm.taobao.org/mirrors/electron/"
```

eg:
```c
//Windows:
npm config set prefix "C:/Program Files/nodejs/npm_global"
npm config set cache "C:/Program Files/nodejs/npm_cache" 

//Linux\Mac:
npm config set prefix "~/nodejs/npm_global"
npm config set cache "~/nodejs/npm_cache"  
```
[淘宝 NPM 镜像](https://npm.taobao.org) 如果你在中国大陆帮助你加速!

从配置的地址或者默认地址，你可以发现 `.npmrc` :
- Windows : `%HOMEPATH%/`
- Linux/Unix/Mac: `~/`  


设置内容如下:
```c
registry=https://registry.npm.taobao.org/
electron_mirror=https://npm.taobao.org/mirrors/electron/
```
#### 4.git克隆项目
```sql
git clone https://github.com/zhuzhuyule/HexoEditor.git
```

#### 5.安装依赖
在mac os系统中, 如果命令`npm install`或者`sudo npm install`失败,你可以使用命令`yarn install`来安装依赖
##### yarn install
```c
yarn install
```
##### npm install
```c
npm install
```
**提示**
```c
//如果发现下载electron失败，你可以尝试运行一下命令
npm install -g electron@1.8.8
```
#### 6.启动
```c
npm start
```
如果使用`yarn`安装依赖，也可以使用一下命令来启动
```
yarn start
```
