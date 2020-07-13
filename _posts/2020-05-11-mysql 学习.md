2.mysql 

binglog日志 记录除了 查询以外的全部操作

relaylog

SHOW MASTER STATUS;

SHOW BINLOG EVENTS IN 'binlog.000021';

# 1.方案

1. 一主一从  主要解决: 热备
2. 一主多从   主要解决:独写分离 高可用 
3. 双主   主要解决:写入压力过大 写分库
4. 级联同步  主要解决:  主库压力过大
5. 环形多主 主要解决: 