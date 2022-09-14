# Burp Suite Crack ja-netfilter.

## Download:

Burp Suite: https://portswigger.net/burp/releases#professional

## How To:

- 将 `config/` 和 `plugins/` 置于 `ja-netfilter.jar` 的同级目录下
- `java -javaagent:ja-netfilter.jar -jar burpsuite_pro_v2022.9.jar` （此时控制台会挂起）
- `java -jar ja-netfilter.jar -r` （另开一个终端执行）
- 按照往常的方式激活
- enjoy!

Credits: Mannix

## 常见问题

### **Java 17+** 报错

增加参数:

```
--add-opens=java.base/jdk.internal.org.objectweb.asm=ALL-UNNAMED
--add-opens=java.base/jdk.internal.org.objectweb.asm.tree=ALL-UNNAMED
```
