In my Project it has multiple microservice. In order to communicate with each other. It uses ApiTemplate for sync communication, but issue is in ApiTemplate we have to mention the IP and port no in URL.
But think of the case where my microservices are deployed in multiple servers. By hardcoding the particular hostname of server, then all request only serve by that server. This leads to increase in load in paricular server of that microservice.
But remaining servers are sitting idle. So, we used this Service Discovey to distribute the load among the microservice servers equally. 
