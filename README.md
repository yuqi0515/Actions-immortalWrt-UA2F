已经全部都正常工作了哦

顺便都加上了ipid

k2p的加上了xray用来科学上网~

如果要自己设置规则记得把
iptables -t mangle -A ua2f -m set --set nohttp dst,dst -j RETURN
改成
iptables -t mangle -A ua2f -m set --match-set nohttp dst,dst -j RETURN


后续弄个刷入即食（大概会弄？）
目前就只加了防火墙方法，其余操作自己来，修改一下ntp，还有开机自启命令就ok了


食用方法：
改test.config里的上面三行，改成自己设备的设置，目前x86，r2s已经测试成功，能正常用
