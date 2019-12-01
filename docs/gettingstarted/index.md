# Getting Started

This [repository](https://github.com/SharePoint/sp-dev-fx-extensions/tree/master/samples) contains community samples that demonstrate different usage patterns for the SharePoint Framework client-side extensions.

Each sample is located in it's own folder with a README.md file that provides details about what it demonstrates and any extra information to help you get the most out of it.

## Using the samples

To build and start using these projects, you'll need to clone and build the projects.

Clone this repo by executing the following command in your console:

```shell
git clone https://github.com/SharePoint/sp-dev-fx-extensions.git
```

Navigate to the cloned repository folder which should be the same as the repository name:

```shell
cd sp-dev-fx-extensions
```

To access the samples use the following command, where you replace `sample-folder-name` with the name of the sample you want to access.

```shell
cd samples
cd sample-folder-name
```

and for the tutorials, use the following command:

```shell
cd tutorials
```

Now run the following command to install the npm packages:

```shell
npm install
```

This will install the required npm packages and dependencies to build and run the client-side project.

Once the npm packages are installed, run the following command to start nodejs to host your extension and preview that in the SharePoint Online pages:

```shell
gulp serve
```

<img src="https://telemetry.sharepointpnp.com/sp-dev-fx-extensions/docs/gettingstarted" />