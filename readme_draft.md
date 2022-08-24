# Actions Runner Controller (ARC)



GitHub Actions is a very useful tool for automating development. GitHub Actions jobs are run in the cloud by default, but you may want to run your jobs in your environment. Self-hosted runner can be used for such use cases, but requires the provisioning and configuration of a virtual machine instance. Instead if you already have a Kubernetes cluster, it makes more sense to run the self-hosted runner on top of it.

`actions-runner-controller` makes that possible. Just create a Runner resource on your Kubernetes, and it will run and operate the self-hosted runner for the specified repository. Combined with Kubernetes RBAC, you can also build simple Self-hosted runners as a Service.
- ✳️ **Deploy your self hosted runners on Kubernetes cluster** like React for writing page templates and layout templates. Turn an existing `.html` or `.liquid` file into a `.jsx` file, and you're off to the componentized races.
- 👥 **Auto scale runners** to insert components into existing pages. Add a line like this to your markdown, HTML, Nunjucks, etc, and watch the magic happen: `{% react 'path/to/component' %}`
- 👥 **Supports Github Enterprise editions** when and how you want. Use component frameworks as a static template to start, and opt-in to shipping JS as needed with our [partial hydration helpers](https://slinkity.dev/docs/partial-hydration/).
- 💅 **Manage** with the power of Vite. Use your favorite CSS preprocessor, JS minifier, and more with minimal config.

> 🚧 Though `actions-runner-controller` is used in production environments, it is still in its early stage of development, hence versioned 0.x. `actions-runner-controller` complies to Semantic Versioning 2.0.0 in which v0.x means that there could be backward-incompatible changes for every release.

The documentation is kept inline with master@HEAD, we do our best to highlight any features that require a specific ARC version or higher however this is not always easily done due to there being many moving parts. Additionally, we actively do not retain compatibly with every GitHub Enterprise Server version nor every Kubernetes version so you will need to ensure you stay current within a reasonable timespan.


## Lets ttry it

The best way to get started is to first read the [ARC overview](https://github.com/actions-runner-controller/actions-runner-controller/blob/master/Actions-Runner-Controller-Overview.md) and then head over to the [Quick start guide](https://github.com/actions-runner-controller/actions-runner-controller/blob/master/QuickStartGuide.md). 🚀



## Learn more

## Contributing

## Troubleshooting
