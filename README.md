## EasyNginxManager

> 顾名思义，就是简单的Nginx管理工具，下文简称`ENM`

`ENM`整体架构分为服务端和客户端，数据交互基于`gRPC`，约定接口为`EasyNginxManagerInterfaces`，下文简称`ENMI`

服务端提供`ENMI`的服务端接口实现和GUI面板以简化人员操作流程

客户端提供`ENMI`的客户端接口实现和BASH执行和IO操作

`ENMI`接口列表

| Interface Name | Request Type | Response Type                   | Run At | Remark         |
| -------------- | ------------ | ------------------------------- | ------ | -------------- |
| ReadConfig     | None         | [NodeConfig](#NodeConfig)       | Client | 读取当前配置   |
| Restart        | None         | [EventResponse](#EventResponse) | Client | 重启Nginx      |
| Start          |              | [EventResponse](#EventResponse) | Client |                |
| Stop           |              | [EventResponse](#EventResponse) | Client |                |
| Status         | None         | [Status](#Status)               | Server | 获取服务端状态 |
|                |              |                                 |        |                |
|                |              |                                 |        |                |
|                |              |                                 |        |                |
|                |              |                                 |        |                |







## Types

### NodeConfig

### EventResponse

### Status
