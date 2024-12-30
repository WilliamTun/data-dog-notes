# Synthetic monitoring

- Testing an application & monitoring it's performance  
- automatically performs actions on applications we believe users/clients will do 


# Monitored metrics
- response times from server to client
- latency - from request to response end
- Load time 
- System & networking resources (CPU, Memory usage)

[ Client ] <---------------------- real request ---------> [ API ]
[ Datadog monitoring client] <---- synthetic request ----> [ API ]

# Use cases
- checks reachability & availability, is our application still up? Is our website online?
- Test new features before launching
- checks performance, Monitor app speed & load times 
- monitor 3rd party services & APIs
- monitor monitor specific issues


### EXAMPLE
- You can simulate post requests to a given API & schedule this in regularly