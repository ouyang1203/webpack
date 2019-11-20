# webpack
## webpack的作用
 ### 1. webpack 能够处理JS文件的相互依赖关系;
 ### 2. webpack 能够处理JS兼容性问题，把高级的，浏览器不识别的语法，转换为较低的浏览器能识别的语法
 ### 3. webpack命令格式为： webpack 要打包的文件路径 -o 打包好输出文件的路径
## 在项目中使用webpack打包
### 注意：main.js是我们所有JS的入口(千万不能使用cnpm安装,否则在npm run dev自动编译时会有莫名其妙的错)
### 1.到项目路径下执行npm init -y初始化项目
### 2.导入jquery终端执行 npm i jquery -s 给项目添加jquery
### 3. 安装webpack
#### npm install webpack-g 安装3.0的webpack或者不指定版本安装最新的npm install webpack -g
#### 安装完毕webpack以后到终端里面执行webpack src/main.js -o dist/bundle.js()
## 使用webpack-dev-server工具来实现自动打包编译的功能
 ### 1. 运行npm install webpack@3.0.0 -D或者npm install webpack -D(不指定版本)把webpack安装到本地项目中
 ### 2. 运行npm i webpack-dev-server@2.11.3 -D 或者 npm i webpack-dev-server -D把这个工具安装到本地项目中
 ### 3. 安装完毕后，这个工具的用法和webpack完全一样
 ### 4. 由于我们是在项目中安装的webpack-dev-server,所以无法直接在powershell终端中运行; (只有全局安装 -g 的工具，终端才能正常执行)
 ### 5. 新的wepack4把weipack-cli分离了，导致webpack-dev-server报错，cnpm i webpack-cli -D就好了
 ### 6. 再次运行npm run dev即可开启自动编译功能，在main.js文件中有修改的时候会自动编译，同时index.html中bundle.js需要改为根目录引用,否则页面查看无效果
