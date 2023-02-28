<H1>Instalación de Mitre Assitant</H1>

<p>Antes de instalar el paquete, actualiza tu sistema operativo<br>
<code>sudo apt update && sudo apt upgrade -y</code></p>

<h3># PRE-REQUISITOS</h3>
<p>- Instalar build-essential<br>
<code>sudo apt install build-essential</code></p>

<p>- Instalar RUST<br>
<code>curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh</code></p>

<h3>Instalar MITRE Assistant</h3>
# Paso 1:
<code>cargo install mitre-assistant</code>
# Step 2:
<code>mitre-assistant download -m enterprise</code>
# Step 3
<code>mitre-assistant baseline -m enterprise</code>
# Comprobamos que funciona:
<code>mitre-assistant -h</code>

Más información:
https://openbase.com/rust/mitre-assistant/documentation
https://docs-ma.vercel.app/docs/project/Brief_Overview
https://www.rust-lang.org/tools/install
