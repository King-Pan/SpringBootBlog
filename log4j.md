1.ConsoleAppender选项 
    Threshold=WARN:指定日志消息的输出最低层次。 
    ImmediateFlush=true:默认值是true,意谓着所有的消息都会被立即输出。 
    Target=System.err：默认情况下是：System.out,指定输出控制台 
2.FileAppender 选项 
    Threshold=WARN:指定日志消息的输出最低层次。 
    ImmediateFlush=true:默认值是true,意谓着所有的消息都会被立即输出。 
    File=mylog.txt:指定消息输出到mylog.txt文件。 
    Append=false:默认值是true,即将消息增加到指定文件中，false指将消息覆盖指定的文件内容。 
3.DailyRollingFileAppender 选项 
    Threshold=WARN:指定日志消息的输出最低层次。 
    ImmediateFlush=true:默认值是true,意谓着所有的消息都会被立即输出。 
    File=mylog.txt:指定消息输出到mylog.txt文件。 
    Append=false:默认值是true,即以追加的方式将消息增加到指定文件中，false指将消息覆盖指定的文件内容。 
    DatePattern=''.''yyyy-ww:每周滚动一次文件，即每周产生一个新的文件。当然也可以指定按月、周、天、时和分。即对应的格式如下: 
    1)''.''yyyy-MM: 每月
    2)''.''yyyy-ww: 每周  
    3)''.''yyyy-MM-dd: 每天 
    4)''.''yyyy-MM-dd-a: 每天两次 
    5)''.''yyyy-MM-dd-HH: 每小时 
    6)''.''yyyy-MM-dd-HH-mm: 每分钟 
4.RollingFileAppender 选项 
    Threshold=WARN:指定日志消息的输出最低层次。 
    ImmediateFlush=true:默认值是true,意谓着所有的消息都会被立即输出。 
    File=mylog.txt:指定消息输出到mylog.txt文件。 
    Append=false:默认值是true,即将消息增加到指定文件中，false指将消息覆盖指定的文件内容。 
    MaxFileSize=100KB: 后缀可以是KB, MB 或者是 GB. 在日志文件到达该大小时，将会自动滚动，即将原来的内容移到mylog.log.1文件。 
    MaxBackupIndex=2:指定可以产生的滚动文件的最大数。 