# Vector Microsar解析，国产MCU适配和自主CP AUTOSAR研发

---
## 联系方式
* 欢迎汽车零部件企业和MCU企业的领导和同仁垂询。
* 联系人：薛女士 
* 联系微信号：CHINCORE2023 
---

## 一、背景介绍
AUTOSAR是由AUTOSAR组织提出的一个开放系统框架，并没有指向任何实际产品。所以，在市场上，众多的第三方企业发布了AUTOSAR协议栈和工具链（以下统称AUTOSAR软件）产品。在国外，VECTOR公司和ETAS公司是AUTOSAR软件行业当之无愧的两大巨头。在国内，从事AUTOSAR软件行业的企业多达十几家，比较大的三家分别是东软睿驰、普华基础软件和经纬恒润。

***众所周知，天下苦AUTOSAR久矣。***

**第一，国外头部企业AUTOSAR软件产品的主要特征是质量可靠、价格昂贵、代码难懂和合作条款限制严格。** 以Vector为例，简单列举如下：其一、Vector是AUTOSAR规范的倡导者和编撰者，进入AUTOSAR软件市场的时机较早，其软件产品有规范且严格的研发流程，又经历大量汽车用户反馈后多轮迭代，已经相对稳定和完善；其二、Vector的Microsar产品清晰易用，文档丰富，满足汽车工程师的日常使用习惯，受到汽车企业的广泛欢迎，但是，其接近垄断的市场地位也造成其软件产品高昂的价格，“大型汽车企业吃不消”和“小型汽车企业消费不起”是不争的事实，Vector事实上是AUTOSAR标准普及的最大赢家之一；其三，Vector的Microsar的协议栈代码高效和简洁，但是，可读性差，几乎没有人能读懂，Davinci Configurator工具链很好用，但是，相关介绍文档太少，汽车工程师不知道软件内部的实施机制；其四、汽车企业只要发生更换主控MCU及工具链、更换量产零部件、更换车型项目等情况都需重新购买整套AUTOSAR软件产品，换而言之，在汽车集团内部的主机厂和零部件企业之间也不能共享其AUTOSAR软件产品，要以部门为单位分开购买以适配不同的零部件产品。

**第二，AUTOSAR软件产品自身也不完善。** 当前，国内外AUTOSAR软件产品是第三方软件公司依据AUTOSAR规范设计，而没有考虑到实际的工程应用情况。举例如下，AUTOSAR软件产品并没有针对不同芯片的内核架构做好完整适配，在软件中存在较多“死循环”等非正常量产状态。

**第三，AUTOSAR软件产品增加汽车工程师的学习成本。在没有AUTOSAR框架时，** 汽车工程师只需要熟悉公司私有协议栈和芯片特性，就可以开发汽车产品。当AUTOSAR发布后，汽车工程师不仅要熟悉原有工作内容，还需要额外理解AUTOSAR的概念。但是，如果新手汽车工程师只理解AUTOSAR概念，那么，当汽车控制器产品内部主控芯片发生异常后，工程师甚至不知道如何定位和调试以解决问题。所以，不少汽车同行称AUTOSAR是新手汽车软件工程师入行的“鸿沟”。

**第四，AUTOSAR软件产品的成本已经不满足当下汽车产业链降本增效的要求。** 过去若干年，在AUTOSAR浪潮推动下，汽车企业逐步在零部件中使用AUTOSAR软件产品替代原有的私有协议栈。然而，在零部件内部都嵌套AUTOSAR软件产品的同质情况下，汽车企业使用AUTOSAR软件产品的优势不复存在，汽车企业之间重新面临激烈的成本竞争。事实上，购买AUTOSAR软件产品的支出均摊到每辆车或每个零部件的固定成本依然较高。所以，有不少汽车产业链的企业在考虑从产品内部移除AUTOSAR软件产品，并启动私有协议栈和工具链的自主研发。但是，这种“返璞归真”的倒车行为将考验工程师的专业软件素质，极大提高软件研发成本，降低软件开发时效，不满足国内汽车行业快速迭代的实际要求。

**最后，以ARM内核为特征的国产车规芯片时代已经来临，** 那么，自主研发AUTOSAR软件也应该尽快提上日程。国产车规芯片ARM内核的生态圈相比以往车规芯片私有内核架构的生态圈更加开放和丰富，汽车工程师有更多的学习资源，也有更广泛的工具链。如果汽车企业仍然坚持购买国外的车规芯片和AUTOSAR软件产品，那么，当前国际形式下供应链断供的风险急剧增加，汽车零部件的成本竞争力也严重下降。所以，拥抱车规芯片的国产化浪潮，在萌芽阶段实施就自主研发AUTOSAR软件产品，实现芯片硬件和AUTOSAR软件的螺旋式迭代，已经是汽车供应链行业内不言自明的共识。

## 二、 基于当前AUTOSAR产品的不足，我司提供三个方面的服务。
### 1. Vector Microsar协议栈和配置工具的解析服务
- 提供Vector Microsar协议栈所有代码的解析服务，包括但不限于，协议栈设计思路，协议栈模块的详细设计文档等。
- 提供Davinci Configurator配置工具内部逻辑的解析服务。
### 2. 国产MCU适配Vector Microsar服务
- 为评估国产MCU的可靠性和耐久性，我司提供Vector Microsar产品在国产MCU的适配服务。帮助MCU企业和汽车供应链企业快速和高效评估国产车规MCU产品的性能。
### 3. 自主AUTOSAR产品的研发服务
- 越来越多的汽车零部件企业期待降本增效，那么，自研AUTOSAR产品是大势所趋。我司提供自主AUTOSAR产品自研过程中的服务，包括但不限于，基于指定公司的AUTOSAR产品，实施协议栈和配置工具重构，实现知识产权的再创新。

### 重点说明： ###
- 更多技术细节，不便在此描述，请现场沟通。
- 由于未获Vector公司授权，我司不提供Microsar的协议栈和Davinci 配置工具。
- 我司暂时只服务与汽车供应链企业和Mcu企业，不向AUTOSAR工具链企业和个人提供服务。

---
## 三、联系方式
* 欢迎汽车零部件企业和MCU企业的领导和同仁垂询。
* 联系人：薛女士 
* 联系微信号：CHINCORE2023 
