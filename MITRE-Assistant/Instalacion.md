<H1>Instalación de Mitre Assitant</H1>

<p>Antes de instalar el paquete, actualiza tu sistema operativo<br>
<code>sudo apt update && sudo apt upgrade -y</code></p>

<h3># PRE-REQUISITOS</h3>
<p>- Instalar build-essential<br>
<code>sudo apt install build-essential</code></p>
<p>- Instalar RUST<br>
<code>curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh</code></p>

<h3># Instalar MITRE Assistant</h3>

<p><strong>Paso 1: Instalar la aplicación</strong><br>
<code>cargo install mitre-assistant</code></p>
<p><strong>Paso 2: Descargar el data set de Mitre ATT&CK</strong><br>
<code>mitre-assistant download -m enterprise</code></p>
<p><strong>Paso 3: Parsear los datos para su tratamiento</strong><br>
<code>mitre-assistant baseline -m enterprise</code></p>
<p><strong>Paso 4: Comprobar que la instalación es correcta</strong><br>
<code>mitre-assistant -h</code></p>

<h3>Más información:</h3>
<div><ul>
<li>https://openbase.com/rust/mitre-assistant/documentation</li>
<li>https://docs-ma.vercel.app/docs/project/Brief_Overview</li>
<li>https://www.rust-lang.org/tools/install</li></ul></div>
