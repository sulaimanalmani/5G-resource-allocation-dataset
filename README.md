# 5G-resource-allocation-dataset
Dataset and resources for 5G network resource allocation models.

# 5G Resource Allocation Dataset

This repository contains the dataset used for training models in the context of 5G network resource allocation. The dataset was collected from our 5G testbed, which consists of a substrate network deployed on a three-node Azure cluster. Below are the details of the testbed and the dataset:

## Testbed Overview

Our 5G testbed includes:

- **RAN:** Implemented using the srsRAN project to create a 3GPP Release 17 compliant gNB and UEs using virtual radios.
- **Core:** Based on Open5GS, with containerized network functions deployed on a Kubernetes cluster.
- **Transport:** Utilizes a VXLAN overlay with Open vSwitch, integrated using the OvS CNI plugin for Kubernetes.

## Dataset Description

The dataset consists of QoS metrics collected from the testbed, with the following parameters:

- **Slice Traffic:** (n_users) Varies from 1 to 5 users/s.
- **Transport Bandwidth Allocation:** (cpu) Ranges from 5 to 40 Mbps.
- **gNB CPU Resource:** (cpu) Ranges from 500 to 4000 millicores.
- **Average Throughput Achieved:** (qos)

## How to Use

You can use the dataset by downloading the `train_dataset` file and integrating it into your machine learning or network optimization models.
