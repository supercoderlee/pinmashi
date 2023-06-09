# 拼码狮（PinMaShi）图形化编程

拼码狮（PinMaShi）是拖拽积木式快速生成Python代码的编程软件。图形化拖拽式编程有效降低编程难度，对Python编程的初学者非常友好；积木式编程加快Python程序的开发，代码使用积木封装加快编程速度；打通硬件间通信实现计算机和智能设备协同编程，一键在本地机器和远程机器调试运行，是Python程序快速开发的利器。PinMaShi采用模块化构建项目工程，通过模块创建工程能够应用在多种场景，例如PC电脑一般程序开发，爬虫项目、物联网项目，树莓派硬件和乐高机器人的远程开发调试，ESP32的python编程应用等。使用PinMaShi将大大简化程序的开发调试过程，积木式编程也更直观更能理解程序逻辑。

## 克隆项目

你需要[Git](https://git-scm.com)工具和[Node.js](https://nodejs.org/en/download/) (包含[npm](http://npmjs.com))克隆到本地才能运行，执行以下命令:

```bash
# 克隆仓库
git clone https://github.com/supercoderlee/pinmashi.git
# 进入目录
cd pinmashi
# 安装依赖
npm install
# 运行应用
npm start
```

## VSCode安装Minify插件

VSCode编辑器安装插件**Minify**插件用于将.js源文件压缩为.min.js版本，项目最终执行的是.min.js文件。

在当前打开的.js文件F1选择Minify即可生成min.js压缩文件，插件设置将Minify Existing On Save项打钩即可保存时自动更新对应的.min.js文件。

## 程序使用方法

运行软件后进入欢迎界面，点击”**开始编程**“进入积木编程界面，此时软件默认使用标准模块创建工程项目。

- **创建项目**：文件菜单中创建项目，选择对应的模块输入项目名称后创建成功，项目将根据模块加载对应的积木。
- **打开和保存项目**：编程项目可以保存为pmsproj文件，并可以再次打开进行编辑。初学者可以在官方资源库(<span>https://github.com/supercoderlee/pinmashi-resources</span>)下载案例进行学习。
- **导入模块**：PinMaShi提供编程平台，具体的应用基于模块来创建，默认提供的标准编程模块基本可以满足一般编程需求，其他特殊的功能如适配硬件、爬虫编程、物联网应用等需要具体的模块来创建。可以在官方资源库（<span>https://github.com/supercoderlee/pinmashi-resources</span>）下载需要的pbmd模块文件导入使用。
- **设备连接**：支持使用IP连接远程设备，例如远程服务器主机、物联网智能设备等，前提是远程机器可以联网能够通过IP进行访问。
- **本地调试**：编写的程序可以在本地或者设备调试，F5键直接本地调试不需要其他复杂操作，前提是本地机器安装了Python解释器。
- **设备调试**：远程设备调试设备将PinMaShi编写的程序F6键上传到设备上运行调试，并且PinMaShi将会监视远程设备执行结果并输出，达到调试和排除问题的目的。另外设备调试还支持远程交互，在本地输入命令将可以控制远程机器。因为需要监视调试结果，每次调试后需要菜单关闭调试（或F7键）手动结束调试。

> **加入交流学习QQ群[647165120](tencent://message/?uin=647165120&Site=&Menu=yes)**
