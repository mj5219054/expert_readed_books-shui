反制攻击队和防守人员
关键词: 反制攻击队/反制攻击方/反制红队/蓝队反制/防守方反制
反制攻击队思路(待完善),提供一些思路,攻击队和防守人员都适用。

    反制攻击队和防守人员
        0x00 开局整牌-给攻击队的环境
        0x01 开局出牌-线上业务
        0x02 开局出牌-其他攻击队线上常涉猎的地方
        0x03 开局出牌-攻击队信息收集阶段的供应链
        0x04 开局出牌-攻击队基础设施
        0x05 开局出牌-攻击队横向移动
        0x06 开局出牌-攻击队线下生活环境
        0x07 开局出牌-人的特性弱点(实施水坑或者其他方式利用)
        0x08 上述部分技术介绍

反制攻击队和防守人员
0x00 开局整牌-给攻击队的环境

目前相关活动从上年开始如火如荼的进行。 反制攻击队要多给攻击队一些甜头，帮助他们渗透，同时也要制造点困难，让攻击队使用复杂攻击手段拿到一个假目标，每当攻击队没思路时，留点后门提示，让攻击队始终在欢喜悲伤交替循环。

具体思路如下： 首先要布置一些入口，让攻击队触发。 待写


内网
0x01 开局出牌-线上业务

例如，把不必要在线上的业务转到内网，保持之前域名解析、网络架构，上线与之前应用开发架构一致的溯源设备。有预算的话，使用与之前业务相同应用，部署真实设备在外网，比如邮箱，要放一些稍微敏感不致命的大量数据，含一些引导信息，引到自己的蜜网，全程流量监控，也要监控流量监控设备（0day打监控设备），与自己网络物理隔离，专人维护，注意保密。有能力的话使用零信任网络，这样在不使用0day情况下，主要突破口会落到有权限的人身上。
0x02 开局出牌-其他攻击队线上常涉猎的地方

文件信息共享（网盘、在线共享网站、贴吧、知乎、微博等）、代码托管（git、码云等）、社交应用（qq、微信、钉钉、电报）、社工裤（论坛、tg）、招聘（脉脉、领英、boos）、有住房信息的平台(酒店、自如、a)、安全信息网站。 github投递exp、钓鱼源码、泄漏敏感信息引导到蜜网。使用蜜罐反制攻击队，比如利用

RMI反序列化
WIN远程连接漏洞CVE-2019-1333
https://paper.seebug.org/1074/
Mysql读文件&反序列化
Dubbo反序列化
NodeJS库rce
Python package 钓鱼
VSCODE EXTENSION 钓鱼
VS Studio 钓鱼
Twitter 钓鱼
恶意vpn
恶意控件
笔记软件rce
社交软件rce
红包插件防撤回插件 钓鱼

解压rce
破解软件 钓鱼
docker客户端 钓鱼
https://www.blackhat.com/docs/us-17/thursday/us-17-Cherny-Well-That-Escalated-Quickly-How-Abusing-The-Docker-API-Led-To-Remote-Code-Execution-Same-Origin-Bypass-And-Persistence.pdf
Xdebug 
Ghidra 钓鱼
bloodhound 漏洞钓鱼
TeamViewer 钓鱼
C2类
Cobalt Strike 漏洞
Cobalt Strike 钓鱼 


[模拟Cobalt Strike上线欺骗入侵者](https://www.cnblogs.com/k8gege/p/12390265.html)
RAT
冰蝎
AWVS 钓鱼

https://github.com/dzonerzy/acunetix_0day
蚁剑
浏览器插件
云盘污染
攻击队打XSS 引诱到蜜罐
GitHub Actions and workflows secure: Preventing pwn requests

https://securitylab.github.com/research/github-actions-preventing-pwn-requests
Packer-Fuzzer工具钓鱼
https://drivertom.blogspot.com/2021/01/packer-fuzzerrce-0day.html
...

安全网站（有个链接总想点,可能养成信息收集习惯）
招聘猎头（很多攻击队是请的外包，会考虑一些岗位，上钩可能性比较大）
0x03 开局出牌-攻击队信息收集阶段的供应链

攻击队常使用fofa（旧版fofa链接处可钓鱼）、钟馗、google、DNSlog平台收集信息，以上可找些洞xss、jsonp、逻辑漏洞收集信息。
信息扫描器 漏洞
0x04 开局出牌-攻击队基础设施

待完善
攻击队为了增加跟踪难度使用开源修改C2 漏洞
攻击队协同办公软件 漏洞
重要节点流量镜像溯源行为，为反制提供信息。
0x05 开局出牌-攻击队横向移动

win登陆认证钓鱼
.PAC网络钓鱼
Ghost potato
路由DNS服务钓鱼
待写
0x06 开局出牌-攻击队线下生活环境

酒店网络
住处(路由器rce、基站)
社交圈(攻击队接触的人)
0x07 开局出牌-人的特性弱点(实施水坑或者其他方式利用)


收集对公司不满的员工，比如论坛，社交微博上的信息等
收集公司人员架构，内部分派，内部矛盾，有些员工出卖其他员工，使其被辞职，不被信任。
先交个朋友，不限男女朋友，建立信任。
外表伪装，年龄小而单纯，眼睛充满迷惑
收集需求，投其所好
转移到有极大权力的组织，借力溯源和起诉攻击者
公司组织内部传递真真假假的信息，只有少数几个人知道哪些是假信息
0x08 上述部分技术介绍

RMI反序列化
由于RMI数据通信大量的使用了Java的对象反序列化，所以在使用RMI客户端去攻击RMI服务端时需要特别小心，如果本地RMI客户端刚好符合反序列化攻击的利用条件，那么RMI服务端返回一个恶意的反序列化攻击包可能会导致我们被反向攻击。

Mysql读文件&反序列化
Mysql client 开启 –enable-local-infile 允许读取客户端文件 http://scz.617.cn:8/network/202001101612.txt http://scz.617.cn:8/network/202005011956.txt
Written on June 5, 2020
