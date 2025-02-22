---
ms.service: azure-monitor
ms.topic: include
ms.date: 10/18/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: Microsoft.Sql/servers/jobAgents, naam
---
<!--
NOTE:  This content is automatically generated using API calls to Azure. 
Any edits made on these files will be overwritten in the next run of the script. 
There is no benefit in editing these files directly.  
-->
  
  
|Metric|Name in REST API|Unit|Aggregation|Dimensions|Time Grains|DS Export|
|---|---|---|---|---|---|---|
|**Elastic Jobs Executions Failed**<p><p>Number of job executions that failed while trying to execute on target |`elastic_jobs_failed` |Count |Total, Count |\<none\>|PT1M |Yes|
|**Elastic Jobs Executions Successful**<p><p>Number of job executions that were able to successfully execute on target |`elastic_jobs_successful` |Count |Total, Count |\<none\>|PT1M |Yes|
|**Elastic Jobs Executions Timed Out**<p><p>Number of job executions that expired before execution was able to finish on target. |`elastic_jobs_timeout` |Count |Total, Count |\<none\>|PT1M |Yes|