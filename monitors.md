# Monitors

- Used for application performance management
- Prevents & reduce risk of incidents


Types of monitors:
1. Host
2. Metric
3. Anomaly : when metrics behave in outlier patterns
4. APM    : Hits, errors, latency
5. Event
6. Forecast
7. Watchdog   : scan all system for anomalies

Once monitors are set up, there is a summary table in "Manage Monitors" tab
which lists all the monitors, their associated tags and the STATUS of each monitor. 

### 1. Hosts
a) Check alerts - triggered when a host stops reporting telemetries 
b) Cluster alerts - when a percentage of hosts in a cluster stops reporting

Choose who to notify: 
eg. emails / slack
+ Create a message for the notification. 

Can create tag for monitor
eg. monitor-type: host
eg. monitor-type: metric

Can put in a priority
eg. P1 (Critical) vs P4 (Low)

### 2. Metric
Detection methods:
1. Threshold alert
2. Change alert
3. Anomaly detection
4. Outlier alert
5. Forecast alert


### 4. APM alert
Choose the scope of the monitor:
- service type
- tag

Set alert thershold:
- warning thresholds 

* can test notifications! 

### 7. Watchdog
Select type:
1. Any APM alert
2. APM error rate
3. APM hits
4. APM latency
