jenkins+docker的持续集成和持续交付,自动触发工程构建和版本发布
持续集成原理
持续集成, 简称CI（continuous integration）.

CI作为敏捷开发重要的一步，其目的在于让产品快速迭代的同时，尽可能保持高质量.
CI一种可以增加项目可见性，降低项目失败风险的开发实践。其每一次代码更新，都要通过自动化测试来检测代码和功能的正确性，只有通过自动测试的代码才能进行后续的交付和部署.
CI 是团队成员间（产研测）更好地协调工作，更好的适应敏捷迭代开发，自动完成减少人工干预，保证每个时间点上团队成员提交的代码都能成功集成的，可以很好的用于对各种WEB、APP项目的打包.
Jenkins

Jenkins
是一个用Java编写的开源的持续集成工具，提供了软件开发的持续集成服务，可监控并触发持续重复的工作，具有开源，支持多平台和插件扩展，安装简单，界面化管理等特点。

jenkins安装

docker 安装jenkins
1、docker pull jenkins
2、docker run --name devops-jenkins -u root -p 8080:8080 -v /opt/data/jenkins_home:/var/jenkins_home -d jenkins

jenkins配置
初始化jenkins及安装插件
启动完jenkins后通过浏览器输入地址http://部署jenkins主机IP:端口
配置信息可以查看这篇博客
https://www.jianshu.com/p/41f2def6ec59

