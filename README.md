dstat
=====
1.支持pidfile参数，并通过pidfile来防止并发执行，可以方便的配置到crontab中。
2.自动记录dstat.log及自动收集元数据dstat_raw.log。
  参数通过—output指定，dstat_raw.log自动根据自动根据log名称生成,–output必需以.log后缀结尾。
3.日志自动归档功能，大于100m，自动归档，归档最多保留2个。
使用示例：
/home/oracle/dbafree/dstat -tydncs --output /home/oracle/dbafree/dstat.log --pidfile /home/oracle/dbafree/dstat.lck --nocolor 10 
更多请参考：http://www.dbafree.net/?p=1166
