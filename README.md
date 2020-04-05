# kubernetes

# Usando Kubernetes in Docker (KinD) para rodar local
## Instalação
curl -Lo ./kind "https://github.com/kubernetes-sigs/kind/releases/download/v0.7.0/kind-$(uname)-amd64"
chmod +x ./kind
sudo mv ./kind /opt/kind
inclua como variavel de ambiente,
ex: adicione no .bashrc: export PATH=$PATH:/opt