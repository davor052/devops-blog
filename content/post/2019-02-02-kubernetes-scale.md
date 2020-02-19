---
title: Scaling My Kubernetes Deployment
date: 2019-02-02
tags: ["kubernetes", "code"]
---
Scaling my Kubernetes deployment
<!--more-->
'''sh
$ kubectl scale deployments/kubernetes-bootcamp --replicas=4
'''
'''sh
$ kubectl get deployments
NAME
DESIRED
kubernetes-bootcamp
4
CURRENT
4
$ kubectl get pods -o wide
NAME
AGE
IP
NODE
kubernetes-bootcamp-5c69669756-9jhz9
3s
172.18.0.7
minikube
kubernetes-bootcamp-5c69669756-lrjwz
3s
172.18.0.5
minikube
kubernetes-bootcamp-5c69669756-slht6
3s
172.18.0.6
minikube
kubernetes-bootcamp-5c69669756-t4pcs
28s
172.18.0.4
minikube
'''
