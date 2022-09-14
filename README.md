# Burp Suite crack after version 2022.9 with ja-netfilter.

[中文版](README.CN.md)

## Download:

Burp Suite: https://portswigger.net/burp/releases#professional

## How To:

- put config/ and plugins/ in same directory of ja-netfilter.jar
- `java -javaagent:ja-netfilter.jar -jar burpsuite_pro_v2022.9.jar`
- `java -jar ja-netfilter.jar -r` (on another window)
- proceed as usual to crack it
- enjoy!

Credits: Mannix

## NOTE:

If you're using the installer version (which has JDK 17+) or JDK 17+ on your own, remember to add this values:
--add-opens=java.base/jdk.internal.org.objectweb.asm=ALL-UNNAMED
--add-opens=java.base/jdk.internal.org.objectweb.asm.tree=ALL-UNNAMED