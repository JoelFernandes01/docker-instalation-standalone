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

#### Esse tutorial foi desenvolvido para criar um ambiente de laboratório/testes com o docker standalone

Dividimos em dois arquivos pequenos e objetivos

[Guia de Instalação do Docker Engine](instalação-docker-engine.md)



#### Docker Compose ####
sudo  curl -SL https://github.com/docker/compose/releases/download/v2.33.1/docker-compose-linux-x86_64 -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
docker compose