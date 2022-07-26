## Introduction

GitHub Actions can be run in GitHub-hosted cloud or self hosted environments. Self-hosted runners offer more control of hardware, operating system, and software tools than GitHub-hosted runners provide

With just a few configurations, you can set up your kubernetes (K8s) cluster to be a self-hosted environment.In this guide, we will deploy Actions Runner controller (ACR) into your K8s cluster, and then target that cluster to run GitHub Action workflows.

## Step 1: Setup your K8s Environment
<details><summary>Setup K8s environment</summary>
If you don't have a K8s environment, you can install a local environment using [minikube]([url](https://minikube.sigs.k8s.io/docs/start/)).
</details>

1. Run the following kubectl command to install certmgr in your environment. For more information, see [certmgr]([url](https://cert-manager.io/docs/installation/))
```yaml{:copy}
kubectl apply -f https://github.com/cert-manager/cert-manager/releases/download/v1.8.2/cert-manager.yaml
```
<sub> This command uses v1.8.2. Please replace with a later version, if available.</sub>

2. Next, we need a Personal Access Token (PAT) for ACR to authenticate with GitHub.
   - Login to GitHub account and Navigate to https://github.com/settings/tokens/new
   - Select  repo
   - Click Generate Token and then copy the token locally ( we’ll need it later) 

👏🏻👏🏻 That’s all the setup we need, next let's deploy and configure ACR


 
