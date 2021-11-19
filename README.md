# express-react-typescript-mongodb

这是一个用于使用Express构建web应用程序的样板工程，并在Typescript的帮助下做出反应。它被配置为将客户端JavaScript和CSS捆绑包以及您的文件作为asset分开。

- express-react-typescript-mongodb
  - 介绍
    - 开发模式
    - 生产模式
  - 快速开始
  - 文档说明
    - 目录结构
    - TODO...


## 介绍

这是一种非常好的配置方法，用于构建具有完整堆栈Typescript的应用程序。它配置为后端开发，使用MongoDB作为数据库，ExpressJS框架用于web服务，前端开发使用ReactJS库，借助Typescript语言和较少的样式表预处理器。

## prerequisite

-首先确保您在某处安装了MongoDB数据库，并更改`src/server/configs.ts`文件中的配置。默认值是localhost。

### 开发模式

在开发模式下，您将有一个后端服务器运行[nodemon](https://nodemon.io/)以及与[webpack dev server]一起运行的前端服务器(https://webpack.js.org/configuration/dev-server/). [网页包开发服务器](https://webpack.js.org/configuration/dev-server/)这有助于前端的热态和动态重新加载。服务器端Express代码将由节点服务器使用[nodemon]提供(https://nodemon.io/)这有助于在服务器端代码更改时自动重新启动服务器。

### 生产模式

在生产模式下，服务器目录中只有后端代码。Webpack将把Typescript和Less加载到JavaScript和CSS包的单独目录中。
将JavaScript与CSS分离有助于浏览器缓存CSS文件。 

## 快速开始

```bash
# Clone the repository
git clone https://github.com/Fractalliter/express-react-typescript <app-name>

#Attention please: change the <app-name> with your prefered name for your app

# Go inside the directory
cd <app-name>

# Install dependencies
yarn (or npm install)

# Start development server
yarn dev (or npm run dev)

# Build for production
yarn build (or npm run build)

# Start production server
yarn start (or npm start)
```

如果你正在寻找typeless和纯css，你可以在这里找到它(https://github.com/crsandeep/simple-react-full-stack)
 
## 文档说明

### 目录结构

后端和前端的源代码将放在src目录中。服务器目录用于web服务，客户端用于开发环境中的UI源代码。对于生产环境，Webpack将客户端目录中的所有内容以及资产中的所有资产文件捆绑到dist目录中。

// TODO...
