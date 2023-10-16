<h1 dir="auto">Instalación de Docker</h1>

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

<h3 dir="auto">Incluir Docker a las fuentes de APT</h3>
<p>Añadir el repositorio de Docker: </p>
<p><code>echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null</code></p>
<p>Actualizar los paquetes de Docker del repositorio recién agregado: <code>sudo apt update</code></p>

<h3 dir="auto">Instalación desde el repositorio de Docker </h3>
<p>Instalación de Docker, Compose y el CLI: <code>sudo apt install docker-ce docker-ce-cli docker-compose containerd.io</code> 
(apt-cache policy docker-ce) </p>
<p>Si todo ha ido bien, este debería ser el resultado:</p>
<p><code>apt-cache policy docker-ce<br>
docker-ce:<br>
  Installed: 5:24.0.6-1~ubuntu.22.04~jammy<br>
  Candidate: 5:24.0.6-1~ubuntu.22.04~jammy<br>
  Version table:<br>
 *** 5:24.0.6-1~ubuntu.22.04~jammy 500<br>
        500 https://download.docker.com/linux/ubuntu jammy/stable amd64 Packages<br>
        100 /var/lib/dpkg/status</code></p>

<h3 dir="auto">Ultimos pasos para dejarlo fino</h3>
<p>Para ejecutar Docker y comandos sin sudo (opcional):</p>
<ul dir="auto">
<li><code>sudo groupadd docker</code></li>
<li><code>sudo usermod -aG docker ${USER}</code></li></ul>

<p>Comprobar que ha ido bien: cerrar la sesión del servidor, volver a iniciarla y comprobar:<code>id -nG</code></p>
<p>Si queremos agregar al grupo docker un usuario con el que no inició sesión, declarar dicho nombre de usuario de forma explícita: <code>sudo usermod -aG docker username</code></p>

<h3 dir="auto">Funcionamiento de Docker</h3>
<ul dir="auto">
<li>Activar o encender el servicio: <code>systemctl start docker</code></li>
<li>Comprobar la instalación de Docker: <code>docker run hello-world</code></li>
<li>Para comprobar el estado del servicio: <code>systemctl status docker</code></li>
<li>Comprobar la instalación de Docker Compose: <code>docker compose version</code></li></ul>
<p>Para ver todos los subcomandos disponibles, escribir lo siguiente: <code>docker</code></p>

<p>Más info:<BR>
<a href=https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04-es#paso-6-administrar-contenedores-de-docker>https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04-es#paso-6-administrar-contenedores-de-docker</a></p>
