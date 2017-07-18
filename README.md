# electronDemo

一个基本的**Electron**应用只需要这些文件：

- `package.json` - 指向应用程序的主文件，并列出其详细信息和依赖关系。
- `main.js` - 启动应用程序并创建一个浏览器窗口来呈现HTML，这是应用程序的**主要进程**。
- `index.html` - 要渲染的网页，这是应用程序的**渲染进程**。

你可以在 [Quick Start Guide](http://electron.atom.io/docs/tutorial/quick-start) 中了解有关这些组件的更多信息。

## 使用

#### 安装依赖
`npm install`
#### 启动app
`npm start`

## 打包

#### 全局安装
`npm install electron-packager -g`

#### 执行打包
`electron-packager . bobo --out ../electron`

- 这段语句表示的意思是把当前文件目录下的资源（.）命名为bobo打包到父级的electron文件夹。

- 此时electron-packager就会自动判别当前的操作系统打包对应的文件，例如windows系统下就会打包成.exe格式。

- 如果你想一次性把所有的操作系统都打包一遍，可以在上面打包语句后面加上-all。

- 由于打包的时候会把浏览器内核完整打包进去，所以就算你的项目开发就几百k的资源，但最终的打包文件估计有40到50M。

## 已有功能

- 黄金比例转换

- RGB与16进制相互转换