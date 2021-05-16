已经全部都正常工作了哦

顺便都加上了ipid

k2p的加上了xray用来科学上网~

iptables -t mangle -A ua2f -m set --set nohttp dst,dst -j RETURN
要改成
iptables -t mangle -A ua2f -m set --match-set nohttp dst,dst -j RETURN

后续弄个刷入即食（大概会弄？）
