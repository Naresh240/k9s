# k9s

## Pre-Requisites

```bash
kubernetes cluster
```

## kubernetes cluster - minikube
[minikube setup](https://github.com/Naresh240/kubernetes/blob/main/minikube-setup/README.md)

## Install k9s

```bash
echo "**** Install k9s *****"

export VERSION_K9S=v0.25.18
curl -LO https://github.com/derailed/k9s/releases/download/${VERSION_K9S}/k9s_Linux_x86_64.tar.gz
tar -xzvf k9s_Linux_x86_64.tar.gz
chmod +x k9s
mv k9s /usr/bin
```

## Check resource with k9s

```bash
k9s                ### crrent namespace
```
![image](https://user-images.githubusercontent.com/58024415/208837437-19426a5c-8d92-4f61-acd6-8f9ade9eef63.png)

```bash
k9s -A             ### All namespaces
```

## Shortcuts

```bash
shift + :         ## To find resources
/                 ## To search specific resource under all resources
d                 ## Description of resource
ctrl + d          ## Delete the resource
ctrl + w          ## Control wide column
```
