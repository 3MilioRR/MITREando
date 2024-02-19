<h1 dir="auto">ATT&amp;CK Navigator</h1>

<p dir="auto">ATT&amp;CK es una herramienta desarrollada en Python, HTML, SCSS y TypeScript.</p>

<p>El uso del navegador es muy amplio: puedes usar el Navigator para hacerte una idea de tu cobertura defensiva, llevar acabo una planificación de tus equipos rojo/azul, la frecuencia de las técnicas detectadas o cualquier otra cosa que quieras hacer. Se integra con nuemerosas herramientas de MITRE y tambien de terceros.</p>
 
<p dir="auto">Existen varias imágenes de Docker que se pueden instalar localmente.</p>
<ol>
<li><a href="https://hub.docker.com/r/sapran/attack-navigator-docker">Sapran</a></li>
<li><a href="https://hub.docker.com/r/bodane/attack-navigator">Bodane</a></li>
<li><a href="https://hub.docker.com/r/vtfoundation/attack-navigator">VT Foundation</a></li>
<li><a href="https://hub.docker.com/r/farwarx/attack-navigator">Farwarx</a></li></ol>

<p dir="auto">Tambien es posible ejecutar una versión on-line, sin necesidad de instalarse nada:<br>
<a href="https://mitre-attack.github.io/attack-navigator/">MITRE Navigator On-line.</a></p>

<h1 dir="auto">Instalación local</h1>
<p dir="auto">Si solo quieres hacer una instalación local, puedes seguir estos pasos:</p>

<p dir="auto"><strong>Requisitos:</strong></p>
<ul dir="auto">
<li><a href="https://nodejs.org/en">Node.js v.18</a></li>
<li><a href="https://angular.io/cli">Angular CLI</a></li></ul>
<p>(Hay una mini guía en esta carpeta para instalar node.js, npm y angular cli)</p>

<p dir="auto"><strong>Instalación</strong></p>
<p>Solo la primera vez:</p>
<ol>
<li>Clona el repositorio de GitHub: <code>git clone https://github.com/mitre-attack/attack-navigator</code></li>
<li>Ve al directorio de nav-app de ATT&CK: <code>cd attack-navigator/nav-app</code></li>
<li>Instala la herramienta con los requisitos: <code>npm install</code></li>
</ol>

<p dir="auto"><strong>Ejecución</strong></p>
<ul dir="auto">
<li>Ve al directorio de DeTT&CT: <code>cd attack-navigator/nav-app</code></li>
<li>Dentro del direcorio nav-app, ejecuta <code>ng serve</code></li>
<li>ATT&CK Navigator debería estar disponible en cualquier navegador (browser) en el puerto 4200: <a href="http://localhost:4200">http://localhost:4200 </a></li> 
</ul>
