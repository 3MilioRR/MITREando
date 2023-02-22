<h1 dir="auto">DeTT&CT</h1>

<p dir="auto">DeTT&CT es una herramienta desarrollada en Python.</p>
<p dir="auto">El framework completo consiste en la propia herramienta, un cliente para la administración de los ficheros YAML, el editor de  DeTT&CT y un juego de tablas para hacer funcionar el entorno.</p>
 
<p dir="auto">Existe una imagen Docker para DeTT&CT, y tambien se puede instalar localmente.</p>

<p dir="auto">Toda la información necesaria para su instalación (docker y offline) está en este enlace:<br>
<a href="https://github.com/rabobank-cdc/DeTTECT/wiki/Installation-and-requirements">https://github.com/rabobank-cdc/DeTTECT/wiki/Installation-and-requirements</a></p>

<strong><h3>Instalación local</strong></h3>
<p dir="auto">Si solo quieres hacer una instalación local, puedes seguir estos pasos:</p>
<p dir="auto"><strong>Requisitos:</strong></p>
<ul dir="auto">
<li>Python 3.8 o superior</li>
<li>pip (gestor de instalación de paquetes de Python)</li>
<li>Instalar con los paquetes del fichero requirements.txt</li></ul>

<p dir="auto"><strong>Instalación</strong></p>
<ol>
<li>Clona el repositorio de GitHub: <code>git clone https://github.com/rabobank-cdc/DeTTECT</code></li>
<li>Ve al directorio de DeTT&amp;CT: <code>cd DeTTECT</code></li>
<li>Instala la herramienta con los requisitos: <code>pip install -r requirements.txt</code></li>
</ol>
<div>
<pre>pip install -r requirements.txt</pre></div>
<clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="pip3 install -r requirements.txt" tabindex="0" role="button" style="display: inherit;">
no sé
</clipboard>

<p dir="auto"><strong>Ejecución</strong></p>
<ul dir="auto">
<li><code>cd DeTTECT</code></li>
<li><code>python3 dettect.py e</code></li>
<li>El editor debería estar disponible en el navegador en el puerto 8080: <a href="http://localhost:8080">http://localhost:8080 </a></li> 
</ul>
