<h1 dir="auto">Instalación de Docker<h1></h1>

<p dir="auto">Una introducción a Dockers:<br>
<a href="https://www.digitalocean.com/community/tutorials/the-docker-ecosystem-an-introduction-to-common-components">https://www.digitalocean.com/community/tutorials/the-docker-ecosystem-an-introduction-to-common-components</a></p>

<h3 dir="auto">Antes de nada</h3>
<p>Comprueba si hay actualizaciones: <code>sudo apt update</code></p>
<p>Actualiza si fuera necesario: <code>sudo apt updgrade</code></p>

<h3 dir="auto">Empezamos</h3>
<p>Instalamos las dependencias: <code>sudo apt install ca-certificates curl gnupg lsb-release</code></p>
<p>Añadimos la clave de GPG para el repositorio oficial de Docker en su sistema: </p>
<ul dir="auto">
<li><code>sudo mkdir -p /etc/apt/keyrings</code></li>
<li><code>curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg</code></li>
<li><code>sudo chmod a+r /etc/apt/keyrings/docker.gpg</code></li></ul>

<h3 dir="auto">Agregue el repositorio de Docker a las fuentes de APT</h3>
<p></p></code>echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

A continuación, actualice el paquete de base de datos con los paquetes de Docker del repositorio recién agregado:
sudo apt update

Asegúrese de estar a punto de realizar la instalación desde el repositorio de Docker en lugar del repositorio predeterminado de Ubuntu:
sudo apt install docker-ce docker-ce-cli docker-compose containerd.io
(apt-cache policy docker-ce)

resultado:
apt-cache policy docker-ce
docker-ce:
  Installed: 5:24.0.6-1~ubuntu.22.04~jammy
  Candidate: 5:24.0.6-1~ubuntu.22.04~jammy
  Version table:
 *** 5:24.0.6-1~ubuntu.22.04~jammy 500
        500 https://download.docker.com/linux/ubuntu jammy/stable amd64 Packages
        100 /var/lib/dpkg/status


Ejecutar el comando Docker sin sudo (opcional)
sudo groupadd docker
sudo usermod -aG docker ${USER}


cierre la sesión del servidor y vuelva a iniciarla o escriba lo siguiente:
id -nG

Si debe agregar al grupo docker un usuario con el que no inició sesión, declare dicho nombre de usuario de forma explícita usando lo siguiente:
sudo usermod -aG docker username

activar o encender el servicio, para ello corre en la terminal la instrucción:
systemctl start docker

Para comprobar el estado del servicio:
systemctl status docker

Comprobar la instalación de Docker
docker run hello-world

Comprobar la instalación de Docker Compose 
docker compose version

Para ver todos los subcomandos disponibles, escriba lo siguiente:
docker



Más info
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04-es#paso-6-administrar-contenedores-de-docker
