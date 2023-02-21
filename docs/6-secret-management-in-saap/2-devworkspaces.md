# Devworkspaces

Built on the open Eclipse Che project, Red Hat OpenShift Dev Spaces uses Kubernetes and containers to provide any member of the development or IT team with a consistent, secure, and zero-configuration development environment. The experience is as fast and familiar as an integrated development environment on your laptop.

Red Hat OpenShift Dev Spaces provides developer workspaces with everything you need to code, build, test, run, and debug applications:

- Project source code
- Web-based integrated development environment (IDE)
- Tool dependencies needed by developers to work on a project
- Application runtime: a replica of the environment where the application runs in production

Pods manage each component of a OpenShift Dev Spaces workspace. Therefore, everything running in a OpenShift Dev Spaces workspace is running inside containers. This makes a OpenShift Dev Spaces workspace highly portable.

Read More at https://access.redhat.com/products/red-hat-openshift-dev-spaces

> Forecastle : https://forecastle-stakater-forecastle.apps.devtest.vxdqgl7u.kubeapp.cloud/

## How to access

A devworkspace is created automatically whenever a new user signs up as discussed in the previous section. In order to access your users devworkspace, do the following steps:

1. Search `devspaces` in search bar at top right corner, Click the URL to devspaces, If prompted Select `Login via Openshift` and Login to cluster.

    ![forecastle-devspaces](images/forecastle-devspaces.png)

2. Click on Workspaces from sidebar, You will see a devworkspace named `<USER_NAME>-<DOMAIN>`, Click on `Open` to open the devworkspace.

    ![devspace-workspace](images/devspace-workspace-pg.png)

3. You will be directed to devworkspace created for your user. 

      ![devspace-homepage](images/devspace-homepage.png)  

## Switch between projects

Gitlab repositories are added as projects in the DevWorkspace.

You can view these projects in bottom left window named `Che (workspace)`. Browse the content by clicking on either of folders.

![devspace-projects](images/devspace-projects.png)

## Accessing the terminal

Open terminal on your DevSpace by pressing `` Ctrl+` `` or clicking Terminal > New Terminal from top menu as highlighted below. 

![devspace-new-terminal](images/devspace-new-terminal.png)

You will be prompted to `Select a container to create a new terminal`. Select `stack-tl500` container, then select working directory, either `stakater-nordmart-review` and `stakater-nordmart-review-ui` as working directory.

![devspace-select-container-for-terminal](images/devspace-select-container-for-terminal.png)


## oc login to cluster

Your user is already logged to the cluster in the devworkspace. 

If you still have any issues, perform the following steps:

1. Find the URL to openshift console via forecastle and Login to the cluster.

    ![forecastle-openshift-console](images/forecastle-openshift-console.png)

2. Hover over the User Name displayed at top right corner of openshift console and select `Copy Login Command` from drop down menu. Click `Display` and copy the oc login command.

    ![console-copy-login-command](images/console-copy-login-command.png)

    ![console-copy-login-command-pg](images/console-copy-login-command-pg.png)
3. Open terminal on your DevSpace by pressing `` Ctrl+` `` or clicking `Terminal > New Terminal` from top menu, Select `stack-tl500` as container, Select working directory. Paste the command copied in the previous step to login.

    ![terminal-oc-login](images/terminal-oc-login.png)

