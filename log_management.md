# Logs

### Log entries contain:
1. Time stamps
2. Type of log: Error / Warn / Info / Debug
3. Additional information - eg. user/api information

### Log management system
gather, process, store and analyse logs from a given system. 

### Purpose:
- pin point areas of poor performance
- assess application health
- diagnose root cause of run time errors

### How to send logs from applications to datadog?
In the code script, add a datadog log object 
& code in the ability to send messages to datadog. 

Note. Different loggers exist for different languages
eg. Logger for python, Logger for Java

Resource: 
https://docs.datadoghq.com/logs/log_collection/python/

### How to see all the logs?
- Go to datadog
- lefthand nav bar - go to "Logs"
- Can filter for logs / search for key words 
