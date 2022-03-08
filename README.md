# Apps
``` pase por aqui CM 
```console
sudo apt install vim ccze htop wget curl unzip openfortivpn -y
```
## INSTALAR KUBECTL
### Descargar la última entrega:
```console
curl -LO "https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl"
```
### Habilita los permisos de ejecución del binario kubectl.
```console
chmod +x ./kubectl
```
### Mueve el binario dentro de tu PATH.
```console
sudo mv ./kubectl /usr/local/bin/kubectl
```
### Comprueba que la versión que se ha instalado es la más reciente.
```console
kubectl version --client
```
## Instalar K9S
```console
curl -sS https://webinstall.dev/k9s | bash
```
### Actualizar el PATH
```console
export PATH="/home/$USER/.local/bin:$PATH"
```
## INSTALAR TERRAFORM

#Descargar la version 0.13.5 o a eleccion
```console
wget https://releases.hashicorp.com/terraform/0.13.5/terraform_0.13.5_linux_amd64.zip
```
### descomprimir
```console
unzip terraform_0.13.5_linux_amd64.zip
```
### Mueve el binario dentro de tu PATH.
```console
sudo mv ./terraform /usr/local/bin/terraform
```
4.- Comprueba que la versión que se ha instalado es la correcta
```console
terraform version
```
## INSTALAR HELM 2
1.- Descargar helm 2
```console
curl -LO https://git.io/get_helm.sh
```
2.- Darle permisos de ejecución
```console
chmod 700 get_helm.sh
```
3.- Ejecutar el script de instalación
```console
./get_helm.sh
```
4.- Comprueba que la versión que se ha instalado es la correcta
```console
helm version
```
## INSTALAR GCLOUD
1.- Descarga del zip de gcloud
```console
wget https://dl.google.com/dl/cloudsdk/channels/rapid/downloads/google-cloud-sdk-364.0.0-linux-x86_64.tar.gz
```
2.- Descomprimir el tar
```console
tar -xzvf google-cloud-sdk-364.0.0-linux-x86_64.tar.gz
```
3.- Instalar 
```console
./google-cloud-sdk/install.sh
```
### Instalacion de Docker y Docker-compose

```console
curl -fsSL https://get.docker.com -o get-docker.sh && sudo sh get-docker.sh
```
```console
sudo apt install docker-compose
```
```console
sudo usermod -aG docker $USER
```
