貌似全部都正常工作了哦

iptables -t mangle -A ua2f -m set --set nohttp dst,dst -j RETURN
要改成
iptables -t mangle -A ua2f -m set --match-set nohttp dst,dst -j RETURN
