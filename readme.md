
> 注：当前项目为 Serverless Devs 应用，由于应用中会存在需要初始化才可运行的变量（例如应用部署地区、函数名等等），所以**不推荐**直接 Clone 本仓库到本地进行部署或直接复制 s.yaml 使用，**强烈推荐**通过 `s init ${模版名称}` 的方法或应用中心进行初始化，详情可参考[部署 & 体验](#部署--体验) 。

# fc-gpt-sovits 帮助文档
<p align="center" class="flex justify-center">
    <a href="https://www.serverless-devs.com" class="ml-1">
    <img src="http://editor.devsapp.cn/icon?package=fc-gpt-sovits&type=packageType">
  </a>
  <a href="http://www.devsapp.cn/details.html?name=fc-gpt-sovits" class="ml-1">
    <img src="http://editor.devsapp.cn/icon?package=fc-gpt-sovits&type=packageVersion">
  </a>
  <a href="http://www.devsapp.cn/details.html?name=fc-gpt-sovits" class="ml-1">
    <img src="http://editor.devsapp.cn/icon?package=fc-gpt-sovits&type=packageDownload">
  </a>
</p>

<description>

FC版GPT-SoVITS项目部署模版

</description>

<codeUrl>

- [:smiley_cat: 应用模版](https://github.com/devsapp/fc-gpt-sovits)
- [:smiley_cat: 镜像代码](https://github.com/zxypro1/GPT-SoVITS)

</codeUrl>
<preview>



</preview>


## 前期准备

使用该项目，您需要有开通以下服务并拥有对应权限：

<service>



| 服务 |  备注  |
| --- |  --- |
| 函数计算 FC |  提供 CPU、GPU 等计算资源 |
| 文件存储 NAS |  存储所需的大模型 |

</service>

<remark>



</remark>

<disclaimers>



</disclaimers>

## 部署 & 体验

<appcenter>
   
- :fire: 通过 [Serverless 应用中心](https://fcnext.console.aliyun.com/applications/create?template=fc-gpt-sovits) ，
  [![Deploy with Severless Devs](https://img.alicdn.com/imgextra/i1/O1CN01w5RFbX1v45s8TIXPz_!!6000000006118-55-tps-95-28.svg)](https://fcnext.console.aliyun.com/applications/create?template=fc-gpt-sovits) 该应用。
   
</appcenter>
<deploy>
    
- 通过 [Serverless Devs Cli](https://www.serverless-devs.com/serverless-devs/install) 进行部署：
  - [安装 Serverless Devs Cli 开发者工具](https://www.serverless-devs.com/serverless-devs/install) ，并进行[授权信息配置](https://docs.serverless-devs.com/fc/config) ；
  - 初始化项目：`s init fc-gpt-sovits -d fc-gpt-sovits`
  - 进入项目，并进行项目部署：`cd fc-gpt-sovits && s deploy -y`
   
</deploy>

## 案例介绍

<appdetail id="flushContent">

通过此模版，可以将[GPT-SoVITS](https://github.com/RVC-Boss/GPT-SoVITS)开源语音生成 / 克隆模型以及WebUI和API服务部署到阿里云函数计算（FC），可用于快速、廉价地制作自己的声音模型以及生成语音。其具有以下特点和功能：

- 零样本文本到语音（TTS）：输入3-10秒的声音样本，即可实现文本到语音的转换，无需大量训练数据。
- 少样本TTS：仅需1分钟的训练数据即可微调模型，提升声音的相似度和真实感。
- 跨语言支持：支持与训练数据集不同语言的推理，目前支持英语、日语和中文。

目前，该项目已在Github获得25.7K star，是一个非常活跃且快速成长的项目。

由于 GPT-SoVITS 需要通过 GPU 算力进行运算，且部署门槛很高，因此借助于 Serverless 开发平台，用户可以简单、方便地将 GPT-SoVITS 部署至函数计算，并享受技术进步带来的技术红利。

</appdetail>

## 使用流程

<usedetail id="flushContent">

应用[快速使用文档](https://www.yuque.com/zxypro/mnayfw/nt5pdxbuukpzfos1)

### 通过WebUI使用

部署成功后，通过`访问域名`即可进入WebUI。

![url](https://img.alicdn.com/imgextra/i2/O1CN015jJ1ZQ1IQIGmxd5Mu_!!6000000000887-0-tps-1468-526.jpg)

![Webui](https://img.alicdn.com/imgextra/i3/O1CN01b50AWD1N6CymnzTGb_!!6000000001520-0-tps-3058-1786.jpg)

### 通过API使用

进入应用详情，找到备注为`GPT-SoVITS API 服务`，名字为`<函数名>__api`的函数，即为API服务函数。具体使用见快速使用文档。

![api](https://img.alicdn.com/imgextra/i4/O1CN01dNkKqJ1IjzIj5GURm_!!6000000000930-0-tps-1752-502.jpg)

</usedetail>

## 注意事项

<matters id="flushContent">
</matters>


<devgroup>


## 开发者社区

您如果有关于错误的反馈或者未来的期待，您可以在 [Serverless Devs repo Issues](https://github.com/serverless-devs/serverless-devs/issues) 中进行反馈和交流。如果您想要加入我们的讨论组或者了解 FC 组件的最新动态，您可以通过以下渠道进行：

<p align="center">  

| <img src="https://serverless-article-picture.oss-cn-hangzhou.aliyuncs.com/1635407298906_20211028074819117230.png" width="130px" > | <img src="https://serverless-article-picture.oss-cn-hangzhou.aliyuncs.com/1635407044136_20211028074404326599.png" width="130px" > | <img src="https://serverless-article-picture.oss-cn-hangzhou.aliyuncs.com/1635407252200_20211028074732517533.png" width="130px" > |
| --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| <center>微信公众号：`serverless`</center>                                                                                         | <center>微信小助手：`xiaojiangwh`</center>                                                                                        | <center>钉钉交流群：`33947367`</center>                                                                                           |
</p>
</devgroup>
