# Devworkspaces

Built on the open Eclipse Che project, Red Hat OpenShift Dev Spaces uses Kubernetes and containers to provide any member of the development or IT team with a consistent, secure, and zero-configuration development environment. The experience is as fast and familiar as an integrated development environment on your laptop.

Red Hat OpenShift Dev Spaces provides developer workspaces with everything you need to code, build, test, run, and debug applications:

- Project source code
- Web-based integrated development environment (IDE)
- Tool dependencies needed by developers to work on a project
- Application runtime: a replica of the environment where the application runs in production

Pods manage each component of a OpenShift Dev Spaces workspace. Therefore, everything running in a OpenShift Dev Spaces workspace is running inside containers. This makes a OpenShift Dev Spaces workspace highly portable.

Read More at https://access.redhat.com/products/red-hat-openshift-dev-spaces

## How to access

A devworkspace is created automatically whenever a new user signs up as discussed in the previous section. In order to access your users devworkspace, do the following steps:

1. Find the URL to openshift console via forecastle and Login to the cluster.

    --- Add Image ---

3. Open the search page from `Home > Search`, Click Resources and search `Devworkspace`. Select `Devworkspace` to show only `Devworkspace` resources. Make sure to change to sandbox project/namespace called `<TENANT_NAME>-<USER_NAME>-<DOMAIN_NAME>-sandbox` on the top bar e.g. if you are registered as rasheed@stakater.com, project name will be `rasheed-rasheed-stakater-sandbox`.

    --- Add Image ---

4. Open the Devworkspace resource in your sandbox namespace and click on yaml. Scroll down to `status` field and look for `mainURL` field. This URL is the link to your provisioned Devsworkspace as part of automation discussed earlier. Open the URL and verify if the Devworkspace is accessible.

    --- Add Image ---

## oc login to cluster

Your user is already logged to the cluster in the devworkspace. If you still have any issues, perform the following steps:

1. Find the URL to openshift console via forecastle and Login to the cluster.

    --- Add Image ---

2. Hover over the User Name displayed at top right corner of openshift console and select `Copy Login Command` from drop down menu. Click `Display` and copy the oc login command.

    --- Add Image ---

3. Open terminal on your DevSpace by pressing Ctrl+Shift+` or clicking Options > Terminal > New Terminal as highlighted below and paste the command copied in the previous step.

    --- Add Image ---

You are now successfully logged into the cluster.

## Switch between projects

We specified the gitlab repositories deployed for your user into our devworkspace as projects. You
