<H1>Instalación de Mitre Assitant</H1>

<p>Antes de instalar el paquete, actualiza tu sistema operativo<br>
<code>sudo apt update && sudo apt upgrade -y</code></p>

<h3># PRE-REQUISITOS</h3>
<p>- Instalar build-essential
sudo apt install build-essential</p>

- Instalar RUST
https://www.rust-lang.org/tools/install
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

Instalar MITRE Assistant
# Step 1:
cargo install mitre-assistant
# Step 2
mitre-assistant download -m enterprise
# Step 3
mitre-assistant baseline -m enterprise
# Comprobamos que funciona:
mitre-assistant -h

Más información:
https://openbase.com/rust/mitre-assistant/documentation
https://docs-ma.vercel.app/docs/project/Brief_Overview
