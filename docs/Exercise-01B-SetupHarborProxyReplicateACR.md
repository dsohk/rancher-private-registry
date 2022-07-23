# Lab 1 B - Setting up Harbor as a proxy to Azure Container Registry (ACR) and replicating images to ACR

In this exercise, we'll continue from the previous step of Lab 1 A. We'll create a new registry endpoint of ACR in Harbor and create a new project for the newly created endpoint and enable Harbor as proxy. 



## Step 1 - Create ACR Endpoint in Harbor

a) Click on `Registries` from the lefst side menu under the **Administration**

![Screenshot-2022-07-22-at-7.34.27-PM-8502921](../images/Screenshot-2022-07-22-at-7.34.27-PM-8502921.png)



b) Click on `+ NEW ENDPOINT` from Registris screen

![Screenshot-2022-07-22-at-7.34.40-PM](../images/Screenshot-2022-07-22-at-7.34.40-PM.png)



c) A pop-up screen will appear to fill in the following details and then click on `TEST CONNECTION`

`Provider : Azure ACR`

`Name : user's choice e.g. rancher-demo-acr-harbor-proxy`

`Endpoint URL : ACR Registry Server Name e.g. https://attendeexx.azurecr.io`

`Access ID : Azure Registry User Name e.g. attendeexx` 

`Access Secret : Azure Registry Password i.e.(system assigned strong password)`

After filling the correct details, you'll receive an inline message `Connection tested successfully` on top of the pop-up window.

![Screenshot-2022-07-22-at-7.35.28-PM](../images/Screenshot-2022-07-22-at-7.35.28-PM.png)



d) Click `OK`  and verify that endpoint is listed. 

![Screenshot-2022-07-22-at-7.35.46-PM](../images/Screenshot-2022-07-22-at-7.35.46-PM.png)

**End of Step 1**



## Step 2 - Replicate container image to ACR

a) Click on `Replications` from the lefst side menu under the **Administration**

![Screenshot-2022-07-23-at-12.33.30-PM](../images/Screenshot-2022-07-23-at-12.33.30-PM.png)

b) Click on `+ NEW REPLICATION RULE` and it will show a pop-up window to fill details.

![Screenshot-2022-07-23-at-12.34.20-PM](../images/Screenshot-2022-07-23-at-12.34.20-PM.png)

c) Fill following details and click on `SAVE`

`Name : as per user's choice e.g. replicate-to-acr`

`Replication method : Push-based`

`Destination registry : select endpoint value from dropdown e.g. rancher-demo-acr-harbor-proxy - https://attendeexx.azurecr.io`

`Trigger Method : Event Based (slect value from dropdown)`

`Delete remote resources when locally deleted : Checked`

![Screenshot-2022-07-23-at-12.35.42-PM](../images/Screenshot-2022-07-23-at-12.35.42-PM.png)



d) Click on radio button of the created rule and click on `REPLICATE`

![Screenshot-2022-07-23-at-1.11.52-PM](../images/Screenshot-2022-07-23-at-1.11.52-PM.png)

e) A confimation message "Do you want to replicate the rule `newly create rule name`?". Click on `REPLICATE`

![Screenshot-2022-07-23-at-1.13.43-PM](../images/Screenshot-2022-07-23-at-1.13.43-PM.png)

Verify that `InProgress` status is shown under **Execution** section. 

![Screenshot-2022-07-23-at-1.20.07-PM](../images/Screenshot-2022-07-23-at-1.20.07-PM.png)

d) After successpul replication, status will be updated to `Succeeded`. Now click on the link under **ID** column. 

![Screenshot-2022-07-23-at-1.21.47-PM](../images/Screenshot-2022-07-23-at-1.21.47-PM.png)

A screen with show the details of replication.

![Screenshot-2022-07-23-at-1.27.31-PM](../images/Screenshot-2022-07-23-at-1.27.31-PM.png)