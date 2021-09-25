
## 一个云编译UA2F固件的项目
###### 已经正常工作了哦，在使用中有任何问题，欢迎反馈给我

* 如果要自己设置规则记得把
<br><code>iptables -t mangle -A ua2f -m set --set nohttp dst,dst -j RETURN</code>
* 改成以下规则
<br><code>iptables -t mangle -A ua2f -m set --match-set nohttp dst,dst -j RETURN</code>


### 食用方法：
##### 用其他设备的话请改Main.config里的上面三行，改成自己所需要的 config，复制别人的来用也行，下面的不要动哦
##### aciton务必使用Main
##### 目前本地编译x86，已测试成功
###### 自己本地编译的话也可以尝试复制Main.config下面那几行进.config里，也能达到效果
