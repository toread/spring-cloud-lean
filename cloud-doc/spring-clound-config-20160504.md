#Spring Cloud Config 定义
简单来说，Spring Cloud Config就是我们通常意义上的配置中心
把应用原本放在本地文件的配置抽取出来放在中心服务器，从而能够提供更好的管理、发布能力。
另外，Spring Cloud Config提供基于以下3个维度的配置管理：
* 应用
    这个比较好理解，每个配置都是属于某一个应用的
* 环境
    每个配置都是区分环境的，如dev, test, prod等
* 版本
    这个可能是一般的配置中心所缺乏的，就是对同一份配置的不同版本管理
    Spring Cloud Config提供版本的支持，也就是说对于一个应用的不同部署实例，
    可以从服务端获取到不同版本的配置，这对于一些特殊场景如：灰度发布，A/B测试等提供了很好的支持。
#如何使用spring cloud config 开发
##概述
<http://nobodyiam.com/images/2016-04-02/overview.png>