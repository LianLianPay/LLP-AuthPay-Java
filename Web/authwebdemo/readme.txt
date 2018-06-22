
            ╭───────────────────────╮
    ────┤           连连支付demo结构说明             ├────
            ╰───────────────────────╯ 
　                                                                  
　       接口名称：连连支付WEB支付(认证支付)
　 　    代码版本：1.0
         开发语言：JAVA-UTF-8
         版    权：连连支付
　       制 作 者：连连支付产业部技术支持组
         联系方式：技术支持服务
        tel：0571-56072616 
        e-mail:guoyx@lianlian.com

    ─────────────────────────────────

───────
 代码文件结构
───────

authpaywebdemo-JAVA-UTF-8
  │
  ├src┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈类文件夹
  │  │
  │  ├com.llpay.client.config
  │  │  │
  │  │  ├PartnerConfig.java┈┈┈┈┈┈商户基础配置类文件
  │  │  │
  │  │  └ServerURLConfig.java┈┈┈┈┈请求服务地址配置类文件
  │  │
  │  ├com.llpay.client.conn
  │  │  │
  │  │  ├CustomHttpClient.java┈┈┈┈┈┈HttpClient类文件
  │  │  │
  │  │  ├HttpRequestSimple.java┈┈┈┈┈HttpClient类文件
  │  │  │
  │  │  └MySSLSocketFactory.java┈┈┈┈┈┈┈HttpClient类文件
  │  │
  │  ├com.llpay.client.enum
  │  │  │
  │  │  ├PayResultEnum.java ┈┈┈┈┈┈┈┈┈支付结果枚举类文件
  │  │  │
  │  │  └SignTypeEnum.java ┈┈┈┈┈┈┈┈┈签名类型枚举类文件
  │  │
  │  ├com.llpay.client.pay
  │  │  │
  │  │  ├InfoQueryServlet.java ┈卡bin信息查询和已绑定信息查询类文件
  │  │  │
  │  │  ├ReceiveNotifyServlet.java ┈┈┈┈┈异步通知接收类文件
  │  │  │
  │  │  └ToPayServlet.java┈┈┈┈构造支付信息类文件
  │  │
  │  ├com.llpay.client.security
  │  │  │
  │  │  ├Base64.java ┈Base64类文件
  │  │  │
  │  │  ├Md5Algorithm.java ┈┈┈┈┈Md5Algorithm类文件
  │  │  │
  │  │  └TraderRSAUtil.java┈┈┈┈TraderRSAUtil类文件
  │  │
  │  ├com.llpay.client.utils
  │  │  │
  │  │  └LLPayUtil.java┈┈┈连连支付工具类文件
  │  │
  │  └com.llpay.client.vo
  │      │
  │      ├OrderInfo.java ┈订单bean
  │      │
  │      ├PayDataBean.java ┈┈┈┈┈异步通知数据bean
  │      │
  │      ├PaymentInfo.java ┈┈┈┈┈支付信息bean
  │      │
  │      └RetBean.java┈┈┈┈异步通知响应bean
  │
  │
  ├WebRoot┈┈┈┈┈┈┈┈┈┈┈┈┈┈页面文件夹
  │  │
  │  ├images┈┈┈┈┈┈┈┈┈图片资源
  │  │
  │  ├about.jsp┈┈┈┈┈┈┈┈┈┈┈连连支付介绍页面
  │  │
  │  ├gotoPlainPay.jsp ┈┈┈┈┈┈┈┈普通接入方式调转连连支付页面文件
  │  │
  │  ├gotoPrepositPay.jsp ┈┈┈┈┈┈卡前置接入方式调转连连支付页面文件
  │  │
  │  ├index.jsp ┈┈┈┈┈┈┈┈demo入口页面
  │  │
  │  ├plainPay.jsp ┈┈┈┈┈┈┈┈普通接入方式页面文件
  │  │
  │  ├prepositPay.jsp ┈┈┈┈┈┈┈┈卡前置接入方式页面文件
  │  │
  │  ├urlReturn.jsp ┈┈┈┈┈┈┈┈页面跳转同步通知文件
  │  │
  │  └WEB-INF
  │       │
  │       └lib（如果JAVA项目中包含这些架包，则不需要导入）
  │          │
  │          ├commons-codec-1.4.jar
  │          │
  │          ├fastjson-1.1.31.jar
  │          │
  │          ├httpclient-4.2.5.jar
  │          │
  │          ├httpclient-cache-4.2.5.jar
  │          │
  │          ├httpcore-4.2.4.jar
  │          │
  │          └httpmime-4.2.5.jar
  │
  └readme.txt ┈┈┈┈┈┈┈┈┈使用说明文本

※注意※
需要配置的文件是：PartnerConfig.java
部署之前需要修改PartnerConfig.java中商户的配置信息，包括安全密钥、商户编号、业务类型等
本代码示例（demo）采用myeclipse工具java servlet语言编写，部署在jboss服务器，部署成功后浏览器中输入
http://ip:port/authpaywebdemo/可以进入demo演示页面。

──────────
 出现问题，求助方法
──────────

如果在集成连连支付接口时，有疑问或出现问题，可在连连支付开放平台上查找答案。
http://open.lianlianpay.com/open/
或者联系我们的技术支持 tel:0571-56072616 




  



