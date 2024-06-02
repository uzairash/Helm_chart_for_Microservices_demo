
# Helm Chart for Microservices Application

This is A helm chart with which you can deploy google Microservices Application on minikube or any other Kubernetes cluster 


## Installation

To deploy the Helm chart with Helmfile follow these steps  

Download latest Binary of helm file which is a tar file, Open the file and change its user permisiions then move the helmfile from the contents of the tar package to /usr/local/bin/

```bash
curl -LO https://github.com/helmfile/helmfile/releases/download/v0.165.0/helmfile_0.165.0_linux_amd64.tar.gz
tar -zxvf helmfile_0.165.0_linux_amd64.tar.gz
chmod +x helmfile
sudo mv helmfile /usr/local/bin/
```

Then deploy the application using helm file
```bash
helmfile apply
```
or 
```bash
helmfile sync
```

Read about the differcne between helmfile apply and sync 
[Here](https://github.com/user/repo/blob/branch/other_file.md)