---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

// Code snippets are only available for the latest version. Current version is 6.x

GraphServiceClient graphClient = new GraphServiceClient(requestAdapter);

com.microsoft.graph.beta.solutions.backuprestore.serviceapps.item.activate.ActivatePostRequestBody activatePostRequestBody = new com.microsoft.graph.beta.solutions.backuprestore.serviceapps.item.activate.ActivatePostRequestBody();
HashMap<String, Object> additionalData = new HashMap<String, Object>();
additionalData.put("effectiveDateTime", "2024-04-19T12-01-03.45Z");
activatePostRequestBody.setAdditionalData(additionalData);
var result = graphClient.solutions().backupRestore().serviceApps().byServiceAppId("{serviceApp-id}").activate().post(activatePostRequestBody, requestConfiguration -> {
	requestConfiguration.headers.add("Authorization", "Bearer <Access-Token>");
});


```