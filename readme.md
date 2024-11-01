
> 注：当前项目为 Serverless Devs 应用，由于应用中会存在需要初始化才可运行的变量（例如应用部署地区、函数名等等），所以**不推荐**直接 Clone 本仓库到本地进行部署或直接复制 s.yaml 使用，**强烈推荐**通过 `s init ${模版名称}` 的方法或应用中心进行初始化，详情可参考[部署 & 体验](#部署--体验) 。

# fc-gpt-sovits-v2 帮助文档

<description>

FC版GPT-SoVITS项目部署模版的V2版更新，推理更快，效果更好。可实现高质量TTS（Text to Speech）文字到语音生成和快速语音克隆。

</description>

<codeUrl>



</codeUrl>
<preview>



</preview>


## 前期准备

使用该项目，您需要有开通以下服务并拥有对应权限：

<service>



| 服务/业务 |  权限  | 相关文档 |
| --- |  --- | --- |
| 函数计算 |  创建函数 | [帮助文档](https://help.aliyun.com/product/2508973.html) [计费文档](https://help.aliyun.com/document_detail/2512928.html) |

</service>

<remark>



</remark>

<disclaimers>



</disclaimers>

## 部署 & 体验

<appcenter>
   
- :fire: 通过 [Serverless 应用中心](https://fcnext.console.aliyun.com/applications/create?template=fc-gpt-sovits-v2) ，
  [![Deploy with Severless Devs](https://img.alicdn.com/imgextra/i1/O1CN01w5RFbX1v45s8TIXPz_!!6000000006118-55-tps-95-28.svg)](https://fcnext.console.aliyun.com/applications/create?template=fc-gpt-sovits-v2) 该应用。
   
</appcenter>
<deploy>
    
- 通过 [Serverless Devs Cli](https://docs.serverless-devs.com/user-guide/install) 进行部署：
  - [安装 Serverless Devs Cli 开发者工具](https://docs.serverless-devs.com/user-guide/install) ，并进行[授权信息配置]( https://docs.serverless-devs.com/user-guide/config) ；
  - 初始化项目：`s init fc-gpt-sovits-v2 -d fc-gpt-sovits-v2`
  - 进入项目，并进行项目部署：`cd fc-gpt-sovits-v2 && s deploy -y`
   
</deploy>

## 案例介绍

<appdetail id="flushContent">

通过此模版，可以将[GPT-SoVITS](https://github.com/RVC-Boss/GPT-SoVITS)开源语音生成 / 克隆模型以及WebUI和API服务部署到阿里云函数计算（FC），可用于快速、廉价地制作自己的声音模型以及生成语音。其具有以下特点和功能：

- 零样本文本到语音（TTS）：输入3-10秒的声音样本，即可实现文本到语音的转换，无需大量训练数据。
- 跨语言支持：支持与训练数据集不同语言的推理，目前支持英语、日语、中文、韩语和粤语。

目前，该项目已在Github获得34.9K star，是一个非常活跃且快速成长的项目。

由于 GPT-SoVITS 需要通过 GPU 算力进行运算，且部署门槛很高，因此借助于 Serverless 开发平台，用户可以简单、方便地将 GPT-SoVITS 部署至函数计算，并享受技术进步带来的技术红利。

</appdetail>

## 使用流程

<usedetail id="flushContent">

应用[快速使用文档](https://www.yuque.com/zxypro/mnayfw/yrvd2gsbvtzbxvnn)

### 通过WebUI使用

部署成功后，通过`访问域名`即可进入WebUI。

![url](https://img.alicdn.com/imgextra/i2/O1CN01NC28Uu1ZqGErC09Az_!!6000000003245-0-tps-1276-534.jpg)

![Webui](https://img.alicdn.com/imgextra/i3/O1CN01xpegSP1HKVhM7mIdJ_!!6000000000739-0-tps-3110-1762.jpg)

### 通过API使用

进入应用详情，找到备注为`GPT-SoVITS API 服务`，名字为`<函数名>__api`的函数，即为API服务函数。具体使用见快速使用文档。

![api](https://img.alicdn.com/imgextra/i4/O1CN01UQsV731Eh0Io9cTqr_!!6000000000382-0-tps-1746-492.jpg)

</usedetail>

## 注意事项

<matters id="flushContent">

本模版目前不包含训练部分内容，只包含推理WebUI和API。

</matters>


<devgroup>


## 开发者社区

您如果有关于错误的反馈或者未来的期待，您可以在 [Serverless Devs repo Issues](https://github.com/serverless-devs/serverless-devs/issues) 中进行反馈和交流。如果您想要加入我们的讨论组或者了解 FC 组件的最新动态，您可以通过以下渠道进行：

<p align="center">  

| <img src="https://img.alicdn.com/imgextra/i2/O1CN010Sk7sv1Xl6WuOb6uU_!!6000000002963-0-tps-666-662.jpg" width="130px" > | <img src="https://img.alicdn.com/imgextra/i4/O1CN010Vt5aw27VN5rJIguB_!!6000000007802-0-tps-668-630.jpg" width="130px" > |
| --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| <center>微信公众号：`serverless`</center>                                                                                         | <center>钉钉交流群：`33947367`</center>                                                                                           |
</p>
</devgroup>
