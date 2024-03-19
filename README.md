# jianmiao_app
简喵APP API 参数解密

版本:5.22.1

整个app逻辑代码都在native层，有xposed检测，检测到有任何开启的xp模块就立马闪退

请求参数有token校验，请求体和返回包使用AES加密，网络请求使用ssl pinning防抓包

# 抓包篇(方法一):
使用HttpCanary抓包，导入证书到系统目录可以直接抓包

# 抓包篇(方法二):
使用Objection抓包

命令1:objection -g com.sicent.app.baba explore

命令2:android root disable

命令3:android sslpinning disable

即可开启代理使用fiddler抓包
# AES解密
加密方式:AES/ECB/PKCS7Padding

key:6h8bngy6y89kgv4h

![image](https://github.com/intAV/jianmiao_app/assets/38396198/0eb1e60f-dc4d-489f-924e-a31d6f03ff6c)

# token校验
待更新
