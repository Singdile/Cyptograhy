### two time pad is insecure
重复使用同一个密钥
![](../Attachment_box/Pasted%20image%2020250630131214.png)


---
### no integrity
不能保证数据完整性。

邮件信息的明文开头格式都是：“From:Bob”，经过加密后变为c。

攻击者知道Bob对应的密文长度，因此将密文对应的Bob与Eve进行XOR操作。

$$p = Bob \oplus Eve$$
$$c'= c \oplus p =  Bob \oplus k \oplus Bob \oplus Eve$$ 
接收者，尝试得到明文.

$$m' = c' \oplus k = Bob \oplus k \oplus Bob \oplus Eve \oplus k$$