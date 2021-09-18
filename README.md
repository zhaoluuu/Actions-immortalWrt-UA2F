已经全部都正常工作了哦

如果要自己设置规则记得把
iptables -t mangle -A ua2f -m set --set nohttp dst,dst -j RETURN
改成
iptables -t mangle -A ua2f -m set --match-set nohttp dst,dst -j RETURN


食用方法：
用其他设备的话请改Main.config里的上面三行，改成自己设备的设置，
aciton务必使用Main
目前x86，r2s已经测试成功，能正常用
