---
title: Azure VMware Solution
geekdocCollapseSection: true
---

## Overview

It is crucial to monitor the resource utilization in order to take timely action. This solution helps in setting up Azure Monitor alerts for Azure VMware Solution Private Cloud. Action owners will receive email notifications if utilization metrics exceeds set threshold.

**Current Version:**  
v1.0.0 (Mar 4, 2024)

## Alerts Table

Table below shows the Alerts configured after the deployment.

| Name                              | Threshold(s) (Severity) | Signal Type        | Frequency       | # Alert Rules |
|-----------------------------------|-------------------------|--------------------|-----------------|---------------|
| CPU Usage per Cluster             | 80 (2)                  | EffectiveCpuAverage| Every 5 minutes | 1             |
| Memory Usage per Cluster          | 80 (2)                  | UsageAverage       | Every 5 minutes | 1             |
| Storage Usage per Datastore       | 70 (2)                  | DiskUsedPercentage | Every 5 minutes | 1             |
| Storage Usage per Datastore (Critical) | 75 (0)            | DiskUsedPercentage | Every 5 minutes | 1             |
| Service Health Alerts             | N/A                     | ServiceHealth      | N/A             | 1             |

## 📣Feedback 📣

Once you've had an opportunity to deploy the solution we'd love to hear from you! Click [here](https://aka.ms/alz/monitor/feedback) to leave your feedback.

If you have encountered a problem please file an issue in our GitHub repo [GitHub Issue](https://github.com/Azure/azure-monitor-baseline-alerts/issues).

## Deployment Guide

We have a [Deployment Guide](./deploy/deploy.md) available for guidance on how to consume the contents of this repo.

## Known Issues

Please see the [Known Issues](Known-Issues).

## Frequently Asked Questions

Please see the [Frequently Asked Questions](../avs/FAQ.md).

## Contributing

This project welcomes contributions and suggestions.
Most contributions require you to agree to a Contributor License Agreement (CLA)
declaring that you have the right to, and actually do, grant us the rights to use your contribution.
For details, visit [https://cla.opensource.microsoft.com](https://cla.opensource.microsoft.com).

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment).
Simply follow the instructions provided by the bot.
You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

{{< hint type=note >}}
Details on contributing to this repo can be found [here](../../../contributing)
{{< /hint >}}

## Telemetry

When you deploy the IP located in this repo, Microsoft can identify the installation of said IP with the deployed Azure resources. Microsoft can correlate these resources used to support the software. Microsoft collects this information to provide the best experiences with their products and to operate their business. The telemetry is collected through customer usage attribution. The data is collected and governed by [Microsoft's privacy policies](https://www.microsoft.com/trustcenter).

If you don't wish to send usage data to Microsoft, or need to understand more about its' use details can be found [here](./Telemetry).

## Trademarks

This project may contain trademarks or logos for projects, products, or services.
Authorized use of Microsoft trademarks or logos is subject to and must follow
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
