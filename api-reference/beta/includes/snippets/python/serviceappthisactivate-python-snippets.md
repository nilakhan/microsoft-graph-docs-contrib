---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

from msgraph_beta import GraphServiceClient
from msgraph_beta.generated.solutions.backup_restore.service_apps.item.activate.activate_request_builder import ActivateRequestBuilder
from kiota_abstractions.base_request_configuration import RequestConfiguration
from msgraph_beta.generated.solutions.backuprestore.serviceapps.item.activate.activate_post_request_body import ActivatePostRequestBody

graph_client = GraphServiceClient(credentials, scopes)

request_body = ActivatePostRequestBody(
	additional_data = {
			"effective_date_time" : "2024-04-19T12-01-03.45Z",
	}
)

request_configuration = RequestConfiguration()
request_configuration.headers.add("Authorization", "Bearer <Access-Token>")


result = await graph_client.solutions.backup_restore.service_apps.by_service_app_id('serviceApp-id').activate.post(request_body, request_configuration = request_configuration)


```