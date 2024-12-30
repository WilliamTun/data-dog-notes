# data-dog-notes
Notes on application and infrastructure monitoring with Data Dog

# Key concepts
- Host
- Agent
- Tags

### 1. Host
- Physical server or VM that is monitored by datadog. 
- We install data dog agents into hosts

E.g 
1. MacOs
2. Debian / Ubuntu
3. Amazon linux
4. AWS lambda 
5. Docker
6. Kubernetes

### 2. Agent
- datadog software that collects events & metrics from hosts
- data is sent back to datadog. 
- A middle layer between an application and datadog website

Agents are composed of TWO componenets:
1. Collector: collects metrics & info from host every 15 seconds
2. Forwarder: sends to datadog via https

Key files:
- Main config file: ../Datadog/datadog.yaml
- Config files for integrations: ../Datadog/conf.d 


Config file contains:
1. data dog API key
2. site of datadog eg. datadoghq.com
3. site proxy
4. hostname 
5. tag

Note. If we edit a datadog config file on a host, you must then restart the agent before the changes take effect.

How do we install an agent? 
On the data dog website, in the left hand nav bar, go to "Integrations". Choose the host type. Then follow the instructions given on datadog hq website for your chosen host. 

### 3. Tags
- add tags to data dog telemetries (collection of metrics)
- Allows us to filter / aggregate metrics of interest 
- Allows us to make rich visualisations 
- eg. staging vs prod tags

================================

# Metrics

3 ways to submit metrics:
1. Agent
2. DogStatsId
3. Datadog HTTP's API

Metric flows:
1. data is collected at specific time intervals
2. collected data is aggregated
3. data is sent to data dog and visualised.

Metric types:
1. Counts: counts X in a given time interval. 
2. Rates: gets the average of X in a given time interval
3. Gauge: snap shot of a given time interval eg. last value submitted within window - as it is sufficient to represent the stream. Used to measure memory or disk space. 
4. Distributions

