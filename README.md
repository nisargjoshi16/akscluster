# Learn Terraform - Provision AKS Cluster

This repo is a companion repo to the [Provision an AKS Cluster learn guide](https://learn.hashicorp.com/terraform/kubernetes/provision-aks-cluster), containing Terraform configuration files to provision an AKS cluster on Azure.


kubernetes_cluster_name = "inviting-tick-aks"
resource_group_name = "inviting-tick-rg"


az aks get-credentials --resource-group inviting-tick-rg --name inviting-tick-aks

az aks browse --resource-group inviting-tick-rg --name inviting-tick-aks


kubectl create secret docker-registry "mytaskappsecret" --namespace "default" --docker-server="todoappazr.azurecr.io" --docker-username="7669b29d-a1f1-4a2a-b8fb-faa8063d5f2d"  --docker-password="ODBPTKFgeP5D80W8Yr-EMXY55Xs1ez_~cK"

