<h2>Tutorial para instalar o docker engine e docker compose </h2>
Esse tutorial foi realizado em um Linux Ubuntu 24.04
<p>Download da ISO do Ubuntu Server</p>
<p>https://mirror.uepg.br/ubuntu-releases/24.04.2/ubuntu-24.04.2-live-server-amd64.iso</p>

<p>Desenvolvido e personalizado por Joel Fernandes</p>
<h2>Meus contatos :</h2>
<p>- Celular:  (61) 98468-1921</p>
<p>- Linkedin: https://www.linkedin.com/in/joel-fernandes-25838425/</p>
<p>- Facebook: https://www.facebook.com/JoelFernandesSilvaFilho/</p>
--------------------------------------------------------------------------
<h3>Esse tutorial foi desenvolvido para criar um ambiente de laboratório/testes com o docker standalone</h3>

## Etapa 1: Faça o clone do repositório em seu Ubuntu 24.04 LTS

````
sudo git  clone https://github.com/JoelFernandes01/zabbix-via-scripts.git
````
![alt text](pictures/gitclone.PNG)

## Etapa 2: Entre na pasta e torne o script executável
![](pictures/chmodZabbix-MySQL-Install.PNG)


# 


Primeira coisa, remover alguma versão que esteja instalado
´´´´
sudo apt autoremove docker.io
´´´´

#### Add Docker's official GPG key:
sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

#### Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "${UBUNTU_CODENAME:-$VERSION_CODENAME}") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
docker --version

#### Docker Compose ####
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
sudo  curl -SL https://github.com/docker/compose/releases/download/v2.33.1/docker-compose-linux-x86_64 -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
docker compose