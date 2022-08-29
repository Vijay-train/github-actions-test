# Actions Runner Controller (ARC)


Github Actions automates the deployment of code to different environments, including production. GitHub Actions can be run in GitHub-hosted cloud or self hosted environments. Self-hosted environments offer more control of hardware, operating system, and software tools than GitHub-hosted runners provide. They can be Self-hosted runners can be physical, virtual, in a container. Containerized environments are lightweight, loosely coupled, highly efficient and can be managed centrally. However, they are not straightforward to use.

`Actions Runner Controller(ARC)` makes it simpler to run self hosted runners on Kubernetes(K8s) managed containers. Just create a Runner resource on your K8s clister, and it will run and operate the self-hosted runner for the specified repository. Combined with Kubernetes RBAC, you can also build simple Self-hosted runners as a Service.

With `ARC` you can : 
- **Deploy your self hosted runners on Kubernetes cluster** with a simple set of commands.
- **Auto scale runners** based on needs.
- **across Github editions** including Github Enterprise editions and Github Enterprise Cloud.
 

> Though `actions-runner-controller` is used in production environments, it is still in its early stage of development, hence versioned 0.x. `actions-runner-controller` complies to Semantic Versioning 2.0.0 in which v0.x means that there could be backward-incompatible changes for every release.

The documentation is kept inline with master@HEAD, we do our best to highlight any features that require a specific ARC version or higher however this is not always easily done due to there being many moving parts. Additionally, we actively do not retain compatibly with every GitHub Enterprise Server version nor every Kubernetes version so you will need to ensure you stay current within a reasonable timespan.


 
# Lets try it

Get up and running with ARC with only a few steps. For more details, refer to [Quick start guide](https://github.com/actions-runner-controller/actions-runner-controller/blob/master/QuickStartGuide.md). 🚀

To understand a high overview of how ARC works, please refer to [Overview](https://github.com/actions-runner-controller/actions-runner-controller/blob/master/Actions-Runner-Controller-Overview.md)



# Learn more

- [Actions Runner controller (Overview)](https://github.com/actions-runner-controller/actions-runner-controller/blob/master/Actions-Runner-Controller-Overview.md)
- [Guides](https://github.com/actions-runner-controller/actions-runner-controller/blob/master/QuickStartGuide.md)
  - Quick Start
  - Managing Access with Groups
  - Automatically scale runners using ACR
  - Using ACR across organizations
- [Authentication](https://github.com/actions-runner-controller/actions-runner-controller#setting-up-authentication-with-github-api)
- [Using Runners with RunnerDeplpyments and](https://github.com/actions-runner-controller/actions-runner-controller#usage)
  - With RunnerDeployments
  - With RunnerSets
- [Automatically scale runners](https://github.com/actions-runner-controller/actions-runner-controller#autoscaling)
  - ..
- [Enterprise support](https://github.com/actions-runner-controller/actions-runner-controller#github-enterprise-support)
  - GHES
  - GHEC
- [Using custom volumes](https://github.com/actions-runner-controller/actions-runner-controller#custom-volume-mounts)
  - With RAM disk
  - NVME SSD
  - Docker Image layer caching
  - Go Module and Build caching
- [Using other runners](https://github.com/actions-runner-controller/actions-runner-controller#alternative-runners)
  - With Docker in Desktop
  - With Kubernetes jobs
- [Other configurations?](https://github.com/actions-runner-controller/actions-runner-controller#runner-labels)
  - Runner labels
  - Runner groups
  - Across organizations


# Contributing
We welcome contributions from the community.For more details on contributing to the project (including requirements) please check out [Getting Started with Contributing](https://github.com/actions-runner-controller/actions-runner-controller/blob/master/CONTRIBUTING.md)

# Troubleshooting
We are very happy to help you with any issues you have. Please check out the [Troubleshooting](https://github.com/actions-runner-controller/actions-runner-controller/blob/master/TROUBLESHOOTING.md) section for common issues.