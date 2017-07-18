# electronDemo

A basic Electron application needs just these files:

- `package.json` - Points to the app's main file and lists its details and dependencies.
- `main.js` - Starts the app and creates a browser window to render HTML. This is the app's **main process**.
- `index.html` - A web page to render. This is the app's **renderer process**.

You can learn more about each of these components within the [Quick Start Guide](http://electron.atom.io/docs/tutorial/quick-start).

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