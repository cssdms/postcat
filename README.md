# Postcat API 客户端（Client）: 二次开发

![Postcat API Client](http://data.eolinker.com/course/QbLMSaJ7f3dcd0b075a7031b31f8acb486e0a090f1bdc8d.jpeg)

<p align="center"><a href="wiki/README.en.md">English</a> | <span>简体中文</span></p>
<p align="center">
  <a href="https://github.com/Postcatlab/postcat"><img src="https://img.shields.io/github/license/Postcatlab/postcat?sanitize=true" alt="License"></a>
  <a href="https://github.com/Postcatlab/postcat/releases"><img src="https://img.shields.io/github/v/release/Postcatlab/postcat?sanitize=true" alt="Version"></a>
  <a href="https://github.com/Postcatlab/postcat/releases"><img src="https://img.shields.io/github/downloads/Postcatlab/postcat/total?sanitize=true" alt="Downloads"></a>
  <a href="https://discord.gg/W3uk39zJCR"><img src="https://img.shields.io/badge/chat-on%20discord-7289da.svg?sanitize=true" alt="Chat"></a>
</p>

## 概述

**Postcat** 是一个强大的开源、免费的、跨平台（Windows、Mac、Linux、Browsers...）的 **API 开发测试工具**，支持 REST、Websocket 等协议（即将支持 GraphQL、gRPC、TCP、UDP），帮助你加速完成 API 开发和测试工作。它非常适合中小团队及个人使用。

![Postcat UI](https://data.eolink.com/ImGzhCi79d0beb5b8221670dffceb61bf642af1960d3881)

我们在保证 **Postcat** 轻巧灵活的同时，还为它设计了一个强大的插件系统，让您可以一键使用插件来增强它的功能。

![Postcat Extensions](https://data.eolink.com/22UMwcV01e087e3549edb91361f15a9ba8047e16d0d3f3f)

因此 **Postcat** 理论上是一个拥有无限可能的 API 产品，可以从Logo 中看到，我们也形象地为它加上了一件披风，代表它的无限可能。

## 免登录在线使用或下载

**Postcat** 现在已经支持 Windows、Mac、Linux等系统，你可以通过以下地址访问并下载。同时我们也提供了 Web 端，方便你在任何浏览器上使用。

**[https://postcat.com/](https://postcat.com//)**

如果您试用之后觉得不错，**请给我们的Postcat一个 Star 和 Fork~**你的支持是我们不断改进产品的动力！

## 详细的文档

[Postcat 文档](https://docs.postcat.com/)

[插件开发文档](https://developer.postcat.com/api/get-started.html)

## 功能特性和迭代计划（Roadmap）

- 🚀 多协议支持

-- 已实现：HTTP REST、Websocket

-- 即将实现：GraphQL、TCP、UDP、gRPC

- 📕 API 文档
- ✨ API 设计
- ⚡ API 测试
- 🎭 Mock
- 🙌 团队协作
- 🎈 文档分享
- 🗺 环境
- 🧶 全局变量
- 🧩 自定义主题风格
- 🌐 多语言支持：中文、English

了解更多具体迭代计划：[Github Project](https://github.com/orgs/Postcatlab/projects/3)
`</br>`也欢迎给我们多多提需求~
`</br>`

## 友情链接

- [APIPark](https://apipark.com?utm_source=postcat) - 专业的API服务平台

## 💪 贡献者 💪

<p align="center">
感谢你们让美好发生！
</p>

<a href="https://github.com/Postcatlab/postcat/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Postcatlab/postcat" />
</a>

<div align="center">
<sub>Power by <a href="https://contrib.rocks">contrib.rocks</a>.</sub>
</div>

## Bug 和需求反馈

如果想要反馈 Bug、提供产品意见，可以创建一个 [Github issue](https://github.com/Postcatlab/postcat/issues) 联系我们，十分感谢！

如果您希望和 Postcat 团队近距离交流，讨论产品使用技巧以及了解更多产品最新进展，欢迎加入以下渠道。

- QQ群号码：981965807
- QQ群链接：[加入Postcat 用户群](https://jq.qq.com/?_wv=1027&k=Kej1qTUy)
- 微信群：

![](http://data.eolinker.com/course/NKhRRF668370911c8b8ea8a0887b5d62e71b0f1a22ad76a.png)

## 开发 Postcat

<details>

<summary>运行代码</summary>

</br>

请确保你已经部署好所需的开发环境：

- Node.js >= 14.17.x
- yarn >= 1.22.x

我们在开发和构建时使用 yarn 作为包管理工具，强烈建议你也这么做，但如果您希望使用 npm 也完全没问题，只是在安装依赖时可能需要多花一些时间。

### 运行桌面端程序

```shell

yarn install

yarn start

```

### 运行浏览器程序

```shell

cd src/browser&&npm install

yarn start

```

### 提高效率

如果想提高开发效率，可以安装 Angular 官方提供的命令行 Angular-cli 快速生成组件、服务等模板。

```

yarn add @angular/cli --global

```

</details>

<details>

<summary>内置命令</summary>

### 运行命令

| 命令                | 描述                                   |
| ------------------- | -------------------------------------- |
| yarn start          | 开发模式下，同时运行在浏览器和桌面端   |
| yarn start:zh       | 中文开发模式，同时运行在浏览器和桌面端 |
| yarn start:web      | 仅运行在浏览器,同时开启后端代理        |
| yarn start:electron | 仅运行在桌面端                         |

> 本项目 i18n 使用的是编译手段，所以开发时无法切换语言

### 打包构建

| 命令            | 描述                     |
| --------------- | ------------------------ |
| sudo yarn build | 各系统打包 Electron 应用 |

### 运行测试

| 命令      | 描述         |
| --------- | ------------ |
| yarn test | 执行单元测试 |

### 常见问题

#### 1. 打包时签名问题，需要修改文件：patches/windowsCodeSign.js 中的参数

#### 2. 若需要签名，需要在windows10中通过powershell命令生成

```powershell

#
# 用于创建postcat项目的windows10 的签名证书文件
#

# 创建自签名证书（有效期 5 年）
$cert = New-SelfSignedCertificate `
  -Subject "OID.1.3.6.1.4.1.311.60.2.1.3=CN, OID.2.5.4.15=Private Organization" `
  -Type CodeSigningCert `
  -KeyUsage DigitalSignature `
  -KeyAlgorithm RSA `
  -KeyLength 2048 `
  -NotAfter (Get-Date).AddYears(5) `
  -CertStoreLocation Cert:\CurrentUser\My

# 验证证书是否生成成功
Get-ChildItem Cert:\CurrentUser\My\$($cert.Thumbprint)


#  导出为 PFX 文件
# 设置 PFX 密码
$password = ConvertTo-SecureString -String "wqkj123" -Force -AsPlainText

# 导出 PFX（包含私钥）
Export-PfxCertificate `
  -Cert "Cert:\CurrentUser\My\$($cert.Thumbprint)" `
  -FilePath "postcat.pfx" `
  -Password $password



# 查找本机的签名证书  名字：  OID.1.3.6.1.4.1.311.60.2.1.3=CN, OID.2.5.4.15=Private Organization
 Get-ChildItem -Recurse Cert: -CodeSigningCert | Select-Object -Property Subject,PSParentPath,Thumbprint | ConvertTo-Json -Compress
```
