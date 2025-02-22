---
ms.service: azure-monitor
ms.topic: include
ms.date: 10/18/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.EventGrid/namespaces, arm
---
<!--
NOTE:  This content is automatically generated using API calls to Azure. 
Any edits made on these files will be overwritten in the next run of the script. 
There is no benefit in editing these files directly.  
-->
  
  
|Metric|Name in REST API|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|**Acknowledge Operations Latency**<p><p>The observed latency in milliseconds for acknowledge events operation. |`AcknowledgeLatencyInMilliseconds` |Milliseconds |Total |`Topic`, `EventSubscriptionName`|PT1M |No|
|**Failed Acknowledged Events**<p><p>The number of events for which acknowledgements from clients failed. |`FailedAcknowledgedEvents` |Count |Total |`Topic`, `EventSubscriptionName`, `Error`, `ErrorType`|PT1M |No|
|**Failed Publish Events**<p><p>The number of events that weren't accepted by Event Grid. This count excludes events that were published but failed to reach Event Grid due to a network issue, for example. |`FailedPublishedEvents` |Count |Total |`Topic`, `Error`, `ErrorType`|PT1M |No|
|**Failed Received Events**<p><p>The number of events that were requested by clients but weren't delivered successfully by Event Grid. |`FailedReceivedEvents` |Count |Total |`Topic`, `EventSubscriptionName`, `Error`, `ErrorType`|PT1M |No|
|**Failed Released Events**<p><p>The number of events for which release failed. |`FailedReleasedEvents` |Count |Total |`Topic`, `EventSubscriptionName`, `Error`, `ErrorType`|PT1M |No|
|**MQTT: Connections**<p><p>The number of active connections in the namespace. |`Mqtt.Connections` |Count |Total |`Protocol`|PT1M |Yes|
|**MQTT: Dropped Sessions**<p><p>The number of dropped sessions by the namespace. |`Mqtt.DroppedSessions` |Count |Total |`DropReason`|PT1M |Yes|
|**MQTT: Failed Published Messages**<p><p>The number of MQTT messages that failed to be published into the namespace. |`Mqtt.FailedPublishedMessages` |Count |Total |`QoS`, `Protocol`, `Error`|PT1M |Yes|
|**MQTT: Failed Routed Messages**<p><p>The number of failed routed messages by the namespace. |`Mqtt.FailedRoutedMessages` |Count |Total |`Error`|PT1M |Yes|
|**MQTT: Failed Subscription Operations**<p><p>The number of failed subscription operations (Subscribe, Unsubscribe). This metric is incremented for every topic filter within a subscription request. |`Mqtt.FailedSubscriptionOperations` |Count |Total |`Protocol`, `OperationType`, `Error`|PT1M |Yes|
|**MQTT: Request Count**<p><p>The number of MQTT requests. |`Mqtt.RequestCount` |Count |Total |`OperationType`, `Protocol`, `Error`, `Result`|PT1M |Yes|
|**MQTT: Successful Delivered Messages**<p><p>The number of messages delivered by the namespace. There are no failures for this operation. |`Mqtt.SuccessfulDeliveredMessages` |Count |Total |`QoS`, `Protocol`|PT1M |Yes|
|**MQTT: Successful Published Messages**<p><p>The number of  MQTT messages that were published successfully into the namespace. |`Mqtt.SuccessfulPublishedMessages` |Count |Total |`QoS`, `Protocol`|PT1M |Yes|
|**MQTT: Successful Routed Messages**<p><p>The number of successful routed messages by the namespace. |`Mqtt.SuccessfulRoutedMessages` |Count |Total |\<none\>|PT1M |Yes|
|**MQTT: Successful Subscription Operations**<p><p>The number of successful subscription operations (Subscribe, Unsubscribe). This metric is incremented for every topic filter within a subscription request. |`Mqtt.SuccessfulSubscriptionOperations` |Count |Total |`Protocol`, `OperationType`|PT1M |Yes|
|**MQTT: Throughput**<p><p>The number of bytes published to or delivered by the namespace. |`Mqtt.Throughput` |Bytes |Total |`Direction`|PT1M |Yes|
|**Publish Operations Latency**<p><p>The observed latency in milliseconds for publish events operation. |`PublishLatencyInMilliseconds` |Milliseconds |Total |`Topic`|PT1M |No|
|**Receive Operations Latency**<p><p>The observed latency in milliseconds for receive events operation. |`ReceiveLatencyInMilliseconds` |Milliseconds |Total |`Topic`, `EventSubscriptionName`|PT1M |No|
|**Reject Operations Latency**<p><p>The observed latency in milliseconds for reject events operation. |`RejectLatencyInMilliseconds` |Milliseconds |Total |`Topic`, `EventSubscriptionName`|PT1M |No|
|**Successful Acknowledged Events**<p><p>The number of events for which delivery was successfully acknowledged by clients. |`SuccessfulAcknowledgedEvents` |Count |Total |`Topic`, `EventSubscriptionName`|PT1M |No|
|**Successful Publish Events**<p><p>The number of events published successfully to a topic or topic space within a namespace. |`SuccessfulPublishedEvents` |Count |Total |`Topic`|PT1M |No|
|**Successful Received Events**<p><p>The total number of events that were successfully returned to (received by) clients by Event Grid. |`SuccessfulReceivedEvents` |Count |Total |`Topic`, `EventSubscriptionName`|PT1M |No|
|**Successful Released Events**<p><p>The number of events that were released successfully by queue subscriber clients. |`SuccessfulReleasedEvents` |Count |Total |`Topic`, `EventSubscriptionName`|PT1M |No|