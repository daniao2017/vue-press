随着SaaS(Software-as-a-Service)的普及，很多客户更倾向于不自己购买服务器等硬件，而是使用软件提供商的统一服务，提供商为不同的客户设置不同的子级域名。
如a.demo.com,b.demo.com 
比如客户A登录他的专属平台a.demo.com，客户B登录他的专属平台b.demo.com，a和b之间互相隔离，互补干涉，使用独立的数据库。

这里结合Laravel聊聊实现过程，抛砖引玉，有更好的方案欢迎讨论

#### 我们的需求：
1. 根据不同域名访问不同数据库
2. 泛域名解析

####  解决1

我们先复杂问题简单化，假设只有两个客户A和B，登录域名已经配好
demo.test 和 lara6.test


#### 讨论：
https://learnku.com/laravel/t/44228

#### 开源类库:
* https://github.com/spatie/laravel-multitenancy
* https://github.com/stancl/tenancy
* https://github.com/tenancy/tenancy


数据库切换：
https://learnku.com/articles/28142
