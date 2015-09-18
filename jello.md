# 基于jello的架构简介

- 整个Web应用由页面组成

<img src="/images/app.png" alt="">

- 页面由组件组成

<img src="/images/page.png" alt="">

- 一个组件一个目录，资源就近维护（组件资源由片段化的css/less/scss images js html/vm/jsp/php/ftl/ json组成）

<img src="/images/templates.png" alt="">

- 项目基本目录

<img src="/images/mulu.png" alt="">

- 如果项目规模较大，涉及多个团队协作，可将具有相关业务功能的页面组织在一起，形成一个子系统，进一步将整个站点拆分出多个子系统来分配给不同团队维护

```
├─common 通用业务子系统
├─user 用户业务子系统   
├─pay 支付业务子系统
├─goods 商品展示子系统   
└─demo 示例系统
```

