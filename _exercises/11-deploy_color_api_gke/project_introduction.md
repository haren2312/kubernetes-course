# Project Introduction: Deploying Color API on Google Kubernetes Engine

Welcome to this exciting project where we’ll deploy our Color API in a managed Google Kubernetes Engine (GKE) cluster! 🎉 In this exercise, our focus will be on bringing together everything we’ve learned about Kubernetes to deploy a functional application using GKE's robust features.

## Overview

In this exercise, you'll implement two environments of our Color API application: a development environment and a production (or "proud") environment. The goal is to deploy version 2.1.0 of the Color API in development, and the stable version 2.0.0 in production. Here are the main steps we'll cover:

1. Create two namespaces: `dev` and `prod`.
2. Deploy MongoDB stateful sets with headless services in each namespace.
3. Set up config maps and secrets for managing configurations and credentials.
4. Create persistent volume claims for MongoDB storage.
5. Configure services, ingresses, and certificates for API access.
6. Implement network policies to control traffic flow between pods.
7. Use `kustomize` to manage customization in deployments.

Before diving into the step-by-step guide, take a moment to try implementing the solution by following the overview steps. It’s a great way to reinforce your learning!

## Step-by-Step Guide

1. **Set Up Namespaces**: Create the `dev` and `proud` namespaces in your GKE cluster.
2. **Deploy MongoDB**: Using the headless service pattern, deploy MongoDB stateful sets in both namespaces.
3. **Handle Configurations**: Configure your application with necessary config maps and secrets for managing sensitive information.
4. **Persistent Storage**: Create persistent volume claims for MongoDB, with differing storage classes for each environment.
5. **Expose the API**: Set up services of type NodePort, and configure ingresses and certificates for external access to the Color API.
6. **Network Policies**: Implement network policies to allow traffic only from the designated pods and create a default policy to deny unwanted traffic.
7. **Customization**: Use `kustomize` to apply specific customizations for each environment, like different ingresses and persistent volume claims.

## Conclusion

Great job! By working through this project, you've taken significant steps to understand how to deploy applications in a Kubernetes environment using GKE. Remember that the key elements we focused on include namespaces, deployments, persistent storage, and network policies. Keep practicing and exploring these concepts, as they’ll be invaluable in your Kubernetes journey! 🚀

---

### Lecture Description

In this lecture, we explore how to deploy the Color API application in a managed Google Kubernetes Engine cluster, focusing on the creation of development and production environments. You will learn to implement Kubernetes features such as namespaces, stateful sets, persistent volumes, and network policies, leveraging GKE's powerful integrations to streamline your deployments.
