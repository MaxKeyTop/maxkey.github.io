---
layout: zh/default
---
<h2>单点注销-Single Logout</h2>
	
单点注销是指用户在一个系统退出后，其所能单点登录访问的所有系统都同时退出。单点注销主要是为提高安全性，避免用户忘记退出所有应用而造成信息的泄密。
    	
    	
IDP支持单点注销(SLO),即用户不仅仅从认证中心注销，同时也注销从认证中心访问的应用系统。	
		
		
其实现方式也非常简单，由于SSO和单点登录的应用都是分开的，使用不同的域名，只是通过认证中心在多个应用系统中传递身份和登录系统。因此，首先注销单点登录应用，然后修改每个应用系统都使用SSO的单点注销页面，SSO的退出页面会将用户登录的Session注销掉。
