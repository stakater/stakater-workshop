# Exercise 6 - SECRET MANAGEMENT 


## 👨‍🍳 Exercise Intro

The purpose of this exercise is to show how secrets are managed in SAAP cluster.

We will be deploying a fictitious application called nordmart-review. This application uses a kubernetes secret.

[Secrets](https://kubernetes.io/docs/concepts/configuration/secret/) Kubernetes objects which contain sensitive data. This sensitive data can be in the form of passwords, keys, tokens, etc. and maybe created independently of your applications and  used in your applications as environment variables or volumes.

In SAAP, we import or fetch secrets externally from vault using external secret operator. 

Let's see this in action.
