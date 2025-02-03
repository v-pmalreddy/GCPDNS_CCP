# Integrating Google Cloud Platform DNS in Microsoft Sentinel
## Introduction
The Google Cloud Platform DNS Codeless Connector for Microsoft Sentinel enables seamless integration of Google Cloud Platform's DNS logs with Microsoft Sentinel without the need for custom code. Developed as part of the Codeless Conector Platform(CCP), this connector simplifies the process of collecting and ingesting DNS query logs and DNS audit logs from Google Cloud Platform into Sentinel.
# Steps to connect
## Step - 1 Install the connector
Install the **Google Cloud Platform DNS** connector from `Content Hub`
## Step - 2 Adding the new Collector
i. After installing the connector, navigate to `Data Connectors` and select on the **Google Cloud Platform DNS** Connector.

ii. A new window pops up in the bottom, and click on `Open Connector Page`. 

iii. Now, click on `Add new collector` button.
## Step - 3 Fill the required details
Navigate to Google Cloud Console and select the project you want to monitor and fetch the following fields

`Project ID` and `Project Number` : You can find these details in the home page of the project.

`GCP subscription name` : If the subscription already exists, you can find this field in the **Pub/Sub** section.

If the subscription does not exists previously, navigate to **Topics** section and create a topic. After creating the Topic, navigate to **Subscriptions** section and create a new subscription by selecting the specific topic.

`Workload Identity Pool ID` : To get this ID, you must run the terraform script for DNS in gshell of Google Cloud Platform. You can find the script files in the home page of the connector or find them in the steps provided below.
### Steps to execute Terrraform scripts
1. [Click here](https://github.com/v-pmalreddy/GCPDNS_CCP/tree/main/GCPDNSLogsSetup) to access the terraform scripts.
2. 
