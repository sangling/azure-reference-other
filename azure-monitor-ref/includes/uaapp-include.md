---
ms.service: azure-monitor
ms.topic: include
ms.date: 08/28/2023
ms.author: edbaynash
author: EdB-MSFT
ms.custom: UAApp
---


| Column | Type | Description |
|---|---|---|
| AppCategory | string |   |
| AppLanguage | string |   |
| AppName | string |   |
| AppOwner | string |   |
| AppType | string |   |
| AppVendor | string |   |
| AppVersion | string |   |
| _BilledSize | real | The record size in bytes |
| Computer | string |   |
| ComputerID | string |   |
| ComputersWithIssues | int |   |
| Guidance | string |   |
| Importance | string |   |
| _IsBillable | string | Specifies whether ingesting the data is billable. When _IsBillable is `false` ingestion isn't billed to your Azure account |
| IsRollup | bool |   |
| Issue | string |   |
| MonthlyActiveComputers | int |   |
| PercentActiveComputers | string |   |
| ReadyForWindows | string |   |
| RollupLevel | string |   |
| SourceSystem | string | The type of agent the event was collected by. For example, `OpsManager` for Windows agent, either direct connect or Operations Manager, `Linux` for all Linux agents, or `Azure` for Azure Diagnostics |
| TestPlan | string |   |
| TestResult | string |   |
| TimeGenerated | datetime |   |
| TotalInstalls | int |   |
| Type | string | The name of the table |
| UpgradeAssessment | string |   |
| UpgradeDecision | string |   |
