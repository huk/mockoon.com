---
title: Requests logging
meta:
  title: Mock API requests logging
  description: Learn how to access requests and responses logs or record your REST API servers calls for easier debugging
order: 90
---

# Requests logging

---

## Accessing the logs

For easier debugging, Mockoon records all entering requests and all the corresponding outgoing responses for each of your mock API. To access an environment's log, click on the "Logs" tab at the top of the window:

![click the logs tab{802x165}](/images/docs/v1.17.0/open-logs.png)

## Logs content

The list shows all intercepted requests and how Mockoon answered to them.
Please note that all requests are intercepted, even the `/favicon` request made by the browser.
Each record contains the entering request and the outgoing response information. This includes the complete list of headers, route params, query params, and body in raw format.

![view the request{790x518}](/images/docs/v1.17.0/logs-request.png)

![view the response{790x518}](/images/docs/v1.17.0/logs-response.png)

The interface is showing truncated bodies for both the request and the response (the truncation length can be adjusted in the settings). You can still view them in full in a separated editor by clicking on **View full body in editor**:

![click on view full body in editor link{790x518}](/images/docs/v1.17.0/logs-response-view-body.png)
![body content is showed in a modal{790x603}](/images/docs/v1.17.0/logs-response-view-body-modal.png)

## Logs metadata

You can also easily see if a request has been caught by Mockoon (record shows a green tick) or has been passed to another URL if the [proxy mode](docs:proxy-mode) is activated (record shows a shield icon):

![view logs metadata{805x479}](/images/docs/v1.17.0/logs-metadata.png)

## Route auto-mocking

Mockoon also offers the possibility to automatically create mocks for entering requests. Click on the "plus" icon on a record to create a route containing the same information (headers, body, etc.):

![create a route from a log{805x479}](/images/docs/v1.17.0/logs-auto-mocking.png)
