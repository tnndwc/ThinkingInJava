# 反向代理

使用反向代理的优势：

+ 隐藏了后端服务器 IP，增加安全性
+ SSL 会话终结在反向代理服务器，后端服务器不必安装证书，这降低了后端服务器的成本开销
+ 在反向代理服务器统一缓存，缓存命中直接返回
+ 静态内容可以直接配置在反向代理服务器中

如果对比 Load Balance，

+ LB 通常是将流量路由到一组相同功能到服务器上（这里着重强调到是：一组）
+ 而反向代理，即便是只有 1 台后台服务器也是有用到，因为反响代理如上所述，提供了诸如：隐藏后端 IP、统一接入 SSL、提供静态内容等功能