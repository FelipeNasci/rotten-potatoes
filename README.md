# rotten-potatoes

## Configuração

MONGODB_DB => Nome do database

MONGODB_HOST => Host do MongoDB

MONGODB_PORT => Posta de acesso ao MongoDB

MONGODB_USERNAME => Usuário do MongoDB

MONGODB_PASSWORD => Senha do MongoDB



## Challenge 2

#### Kubernets Deploy

- page

![Kubernets Deploy](https://github.com/FelipeNasci/rotten-potatoes/blob/main/images/kubernets-deploy.PNG?raw=true)

#### Setup

- K3D

```bash
choco install k3d
```

- kubernetes-cli

```bash
choco install kubernetes-cli
```

#### Scripts

- Create Cluster

```bash
k3d cluster create kube-cluster --servers 3 --agents 3 -p "8080:30000@loadbalancer"
```
- Run deployment

```bash
kubectl apply -f k8s/deployment.yaml
```

## Challenge 3

#### Kubernets Deploy

- page

![github-actions](https://github.com/FelipeNasci/rotten-potatoes/blob/main/images/github-actions.jpg?raw=true)
