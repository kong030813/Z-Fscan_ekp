# Z-Fscan_ekp
fscan二开，增加一些扫描完内网常见漏洞后的利用，方便被应急响应后还有其他机器在线  
在实战内网中,可能一扫蓝队就应急响应，还没搭隧道获取其他机器权限入口点就已经断网或者下线,  
此项目可以利用常见的内网漏洞快速执行命令，扫描到出网机器直接上线到vshell或者supershell等c2上，防止入口点丢失（默认执行ifconfig，就算断网也有截图得路径分）  
mssql模块 -mc 执行命令   
xp_cmdshell已支持  
<img width="656" alt="图片" src="https://github.com/kong030813/Z-Fscan_ekp/assets/97926809/15f6fb38-e2a6-4321-a3c7-962c123577cf">  
redis模块 -rw 直接写入公钥，-c指定命令（默认ifconfig）   
<img width="646" alt="图片" src="https://github.com/kong030813/Z-Fscan_ekp/assets/97926809/31193f9a-2b87-48c9-8de6-002a9f2d939c">  

后续计划更新  
支持clr mssql命令执行  
对扫描结果进行分类存储方便观看  
