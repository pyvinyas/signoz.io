---
title: Logs SigNoz Cloud Troubleshooting
id: logs-troubleshooting
---

These are instructions for logs troubleshooting for SigNoz Cloud.

### Q. In java my mdc attributes are not visible in SigNoz

It’s present in this [documentation](https://signoz.io/docs/userguide/collecting_application_logs_otel_sdk_java) 
`otel.instrumentation.logback-appender.experimental.capture-mdc-attributes=*`  for **logback** and `otel.instrumentation.log4j-appender.experimental.capture-mdc-attributes=*` for **log4j**

### Q. I want to extract trace_id and span_id from my log line

You can extract these using the logs pipelines trace parser - documentation [here](https://signoz.io/docs/logs-pipelines/guides/trace/)

### Q.I want to extract a attribute from my log line

The best way to do this is using Logs Pipeline. You can follow these two Docs: 
- [Logs Pipeline Introductions](https://signoz.io/docs/logs-pipelines/introduction/)
- [Parse JSON logs with Pipelines](https://signoz.io/docs/logs-pipelines/guides/json/)


### Q. I am sending logs but my logs are not visible on SigNoz

Check by adding a console exporter on application level if you are using SDK else on a local collector level.
Once the above is checked and if you are still facing issue then reach out to us on Intercom - the chatbox at the bottom right corner of your SigNoz Cloud interface.


### Q. How to increase the retention period of logs from x days to y days?
Reach out to us on Intercom - the chatbox at the bottom right corner of your SigNoz Cloud interface.
