---
ms.service: azure-monitor
ms.topic: include
ms.date: 10/18/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.Network/applicationgateways, naam
---
<!--
NOTE:  This content is automatically generated using API calls to Azure. 
Any edits made on these files will be overwritten in the next run of the script. 
There is no benefit in editing these files directly.  
-->
  
  
|Metric|Name in REST API|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|**Application Gateway Total Time**<p><p>Time that it takes for a request to be processed and its response to be sent. This is the interval from the time when Application Gateway receives the first byte of an HTTP request to the time when the response send operation finishes. It's important to note that this usually includes the Application Gateway processing time, time that the request and response packets are traveling over the network and the time the backend server took to respond. |`ApplicationGatewayTotalTime` |MilliSeconds |Average, Maximum |`Listener`|PT1M |No|
|**Requests per minute per Healthy Host**<p><p>Average request count per minute per healthy backend host in a pool |`AvgRequestCountPerHealthyHost` |Count |Average |`BackendSettingsPool`|PT1M |No|
|**WAF Bot Protection Matches**<p><p>Matched Bot Rules |`AzwafBotProtection` |Count |Total |`Action`, `Category`, `Mode`, `CountryCode`, `PolicyName`, `PolicyScope`|PT1M |Yes|
|**WAF Custom Rule Matches**<p><p>Matched Custom Rules |`AzwafCustomRule` |Count |Total |`Action`, `CustomRuleID`, `Mode`, `CountryCode`, `PolicyName`, `PolicyScope`|PT1M |Yes|
|**WAF Managed Rule Matches**<p><p>Matched Managed Rules |`AzwafSecRule` |Count |Total |`Action`, `Mode`, `RuleGroupID`, `RuleID`, `CountryCode`, `PolicyName`, `PolicyScope`, `RuleSetName`|PT1M |Yes|
|**WAF Total Requests**<p><p>Total number of requests evaluated by WAF |`AzwafTotalRequests` |Count |Total |`Action`, `CountryCode`, `Method`, `Mode`, `PolicyName`, `PolicyScope`|PT1M |Yes|
|**Backend Connect Time**<p><p>Time spent establishing a connection with a backend server |`BackendConnectTime` |MilliSeconds |Average, Maximum |`Listener`, `BackendServer`, `BackendPool`, `BackendHttpSetting`|PT1M |No|
|**Backend First Byte Response Time**<p><p>Time interval between start of establishing a connection to backend server and receiving the first byte of the response header, approximating processing time of backend server |`BackendFirstByteResponseTime` |MilliSeconds |Average, Maximum |`Listener`, `BackendServer`, `BackendPool`, `BackendHttpSetting`|PT1M |No|
|**Backend Last Byte Response Time**<p><p>Time interval between start of establishing a connection to backend server and receiving the last byte of the response body |`BackendLastByteResponseTime` |MilliSeconds |Average, Maximum |`Listener`, `BackendServer`, `BackendPool`, `BackendHttpSetting`|PT1M |No|
|**Backend Response Status**<p><p>The number of HTTP response codes generated by the backend members. This does not include any response codes generated by the Application Gateway. |`BackendResponseStatus` |Count |Total |`BackendServer`, `BackendPool`, `BackendHttpSetting`, `HttpStatusGroup`|PT1M |Yes|
|**Web Application Firewall Blocked Requests Rule Distribution**<p><p>Web Application Firewall blocked requests rule distribution |`BlockedCount` |Count |Total |`RuleGroup`, `RuleId`|PT1M |Yes|
|**Bytes Received**<p><p>The total number of bytes received by the Application Gateway from the clients |`BytesReceived` |Bytes |Total |`Listener`|PT1M |Yes|
|**Bytes Sent**<p><p>The total number of bytes sent by the Application Gateway to the clients |`BytesSent` |Bytes |Total |`Listener`|PT1M |Yes|
|**Current Capacity Units**<p><p>Capacity Units consumed |`CapacityUnits` |Count |Average |\<none\>|PT1M |No|
|**Client RTT**<p><p>Round trip time between clients and Application Gateway. This metric indicates how long it takes to establish connections and return acknowledgements |`ClientRtt` |MilliSeconds |Average, Maximum |`Listener`|PT1M |No|
|**Current Compute Units**<p><p>Compute Units consumed |`ComputeUnits` |Count |Average |\<none\>|PT1M |No|
|**CPU Utilization**<p><p>Current CPU utilization of the Application Gateway |`CpuUtilization` |Percent |Average |\<none\>|PT1M |No|
|**Current Connections**<p><p>Count of current connections established with Application Gateway |`CurrentConnections` |Count |Total |\<none\>|PT1M |Yes|
|**Estimated Billed Capacity Units**<p><p>Estimated capacity units that will be charged |`EstimatedBilledCapacityUnits` |Count |Average |\<none\>|PT1M |No|
|**Failed Requests**<p><p>Count of failed requests that Application Gateway has served |`FailedRequests` |Count |Total |`BackendSettingsPool`|PT1M |Yes|
|**Fixed Billable Capacity Units**<p><p>Minimum capacity units that will be charged |`FixedBillableCapacityUnits` |Count |Average |\<none\>|PT1M |No|
|**Healthy Host Count**<p><p>Number of healthy backend hosts |`HealthyHostCount` |Count |Average |`BackendSettingsPool`|PT1M |Yes|
|**Web Application Firewall Total Rule Distribution**<p><p>Web Application Firewall Total Rule Distribution for the incoming traffic |`MatchedCount` |Count |Total |`RuleGroup`, `RuleId`|PT1M |Yes|
|**New connections per second**<p><p>New connections per second established with Application Gateway |`NewConnectionsPerSecond` |CountPerSecond |Average |\<none\>|PT1M |No|
|**Response Status**<p><p>Http response status returned by Application Gateway |`ResponseStatus` |Count |Total |`HttpStatusGroup`|PT1M |Yes|
|**Throughput**<p><p>Number of bytes per second the Application Gateway has served |`Throughput` |BytesPerSecond |Average |\<none\>|PT1M |No|
|**Client TLS Protocol**<p><p>The number of TLS and non-TLS requests initiated by the client that established connection with the Application Gateway. To view TLS protocol distribution, filter by the dimension TLS Protocol. |`TlsProtocol` |Count |Total |`Listener`, `TlsProtocol`|PT1M |Yes|
|**Total Requests**<p><p>Count of successful requests that Application Gateway has served |`TotalRequests` |Count |Total |`BackendSettingsPool`|PT1M |Yes|
|**Unhealthy Host Count**<p><p>Number of unhealthy backend hosts |`UnhealthyHostCount` |Count |Average |`BackendSettingsPool`|PT1M |Yes|