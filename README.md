1：2019年新版本的spring cloud框架（boot2，springgateway）
2：eureka集群
3：springgateway采用动态路由，不停应用加服务，通过redis共享路由信息，方便实现gateway集群
4：框架内，client1和client2是同一个服务名称的web服务，是您的企业应用前台，通过springgateway负载均衡。
5：所有框架内的web服务均实现SSO，权限认证交sso-server项目，把security安全对象单点登陆交给与client1，2项目
无登陆权限的网关访问均被拦截到SSO统一登陆页面。
6：resource项目是演示如何通过web页面和postman方式通过Oauth2协议访问资源服务器
7：client1和client2项目有代码注释，提示你实现session管理（注销session，session安放security对象）
亮点：升级到最新的微服务框架，坑很多，当SSO遇上spring gateway，问题更加多。
http://127.0.0.1:8082/uaa/authentication/require --统一登陆前台
另外还分享一套后台管理系统，基于微服务框架，前台采用VUE的webpack流程开发，精美漂亮。
联系QQ：1075228562
源码（含注释）的获取地址：链接: https://pan.baidu.com/s/1lqbATzEEKmUUecdjDnsN7w 提取码: fim8 
解压密码：https://www.xiaocifang.com/i/EP7c1708630HA.html
