# Deploying tradefinance app to GKE via Google Cloud Marketplace

## Overview
tradefinance is a application for document automation, i.e. extraction of entities from digital documents.

The 
[Google Cloud Marketplace][1] 
is a easy way to deploy apps like tradefinance to a 
[Google Kubernetes Engine][2] 
cluster, with just a few clicks.

[1]: https://console.cloud.google.com/
[2]: https://cloud.google.com/kubernetes-engine/
## Installation

### Quick install with Google Cloud Marketplace

Deploy tradefinance to Google Kubernetes Engine using Google Cloud Marketplace, by following the [on-screen instructions.]()

### Command line instructions

```sh
export TAG="1.0"
export TF_MP_NAMESPACE="tf-app-namespace"
export TF_MP_TLD="example.com"
export GCR_REGISTRY="https://console.cloud.google.com/gcr/images/cloud-marketplace/GLOBAL/tf-public/tradefinance/deployer:${TAG}"
export TF_MP_PARAMS="{\"APP_INSTANCE_NAME\": \"${TF_MP_APP_INSTANCE_NAME}\",\"NAMESPACE\": \"${TF_MP_NAMESPACE}\", \"global.hosts.domain\": \"${TF_MP_TLD}\"}"

```
