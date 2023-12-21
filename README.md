# Kubernetes Namespace Lister (k8s-ns-list)

## Overview
The Kubernetes Namespace Lister (`k8s-ns-list`) is a simple CLI tool written in Go for learning purposes. It just provides a quick way to list all the namespaces in a Kubernetes cluster. This tool is intended for those getting started with K8s and `kubectl`, offering an introduction to building CLI tools that interact with the Kubernetes API.

## Prerequisites
- Go version 1.11 or higher.
- Access to a Kubernetes cluster and a configured `kubeconfig` file.

## Installation

1. **Clone the Repository**

   ```
   git clone https://github.com/hariscats/k8s-namespace-list.git
   cd k8s-namespace-list
   ```

2. **Build the Tool**

   ```
   cd cmd/
   go build -o k8s-ns-list
   ```

3. **(Optional) Install the Binary**

   Move the binary to a directory in your `PATH` to run it from anywhere:

   ```
   mv k8s-ns-list /usr/local/bin
   ```

## Usage

Run the tool to list all namespaces in your Kubernetes cluster:

```
./k8s-ns-list
```

To specify a kubeconfig file:

```
./k8s-ns-list --kubeconfig=/path/to/kubeconfig
```