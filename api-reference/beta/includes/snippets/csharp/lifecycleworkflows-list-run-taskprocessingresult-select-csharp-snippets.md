---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var taskProcessingResults = await graphClient.IdentityGovernance.LifecycleWorkflows.Workflows["{identityGovernance.workflow-id}"].Runs["{identityGovernance.run-id}"].TaskProcessingResults
	.Request()
	.Select("id,failureReason,processingStatus,subject")
	.GetAsync();

```