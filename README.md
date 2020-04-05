# kubernetes

# Usando Kubernetes in Docker (KinD) para rodar local
## Instalação
curl -Lo ./kind "https://github.com/kubernetes-sigs/kind/releases/download/v0.7.0/kind-$(uname)-amd64"
chmod +x ./kind
sudo mv ./kind /opt/kind
inclua como variavel de ambiente,
ex: adicione no .bashrc: export PATH=$PATH:/opt

# Instalação Minikube
- Instale o kubectl:
curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl

chmod +x ./kubectl

sudo mv ./kubectl /usr/local/bin/kubectl

kubectl version --client

curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64 \
  && chmod +x minikube

sudo mv ./minikube /usr/local/bin/minikube

minikube version

minikube start --driver=<driver_name>
experimente o driver docker

minikube status