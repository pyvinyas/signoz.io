---
title: Logs SigNoz Cloud Troubleshooting
id: logs-troubleshooting
---

These are instructions for logs troubleshooting for SigNoz Cloud.

Q. In java my mdc attributes are not visible in signoz
A.It’s present in this doc https://signoz.io/docs/userguide/collecting_application_logs_otel_sdk_java
otel.instrumentation.logback-appender.experimental.capture-mdc-attributes=*  for logback and otel.instrumentation.log4j-appender.experimental.capture-mdc-attributes=* for log4j

Q. I want to extract trace_id and span_id from my log line

A.use pipelines trace parser https://signoz.io/docs/logs-pipelines/guides/trace/

Q.I want to extract a attribute from my log line
A. https://signoz.io/docs/logs-pipelines/introduction/
https://signoz.io/docs/logs-pipelines/guides/json/

Q. I am sending logs but my logs are not visible on signoz
A. Check by adding a console exporter (on application level if they are using SDK else on a local collector level)
Once the above is checked and the user is still facing issue then reach out to us.
