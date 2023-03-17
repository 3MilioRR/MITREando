<h1 dir="auto">FLOW ATT&CK</h1>

<h3 dir="auto">Ejecutar Flow ATT&CK on-line (online builder)</h3>
<p dir="auto"><a href="https://center-for-threat-informed-defense.github.io/attack-flow/ui/">https://center-for-threat-informed-defense.github.io/attack-flow/ui/</a></p>

<h3 dir="auto">Ejecutar Flow ATT&CK en la máquina virtual</h3>
<p dir="auto">Arrancar el docker: <code>docker start AttackFlowBuilder</code><br>
Visualizar en el navegador: <code><a href="localhost:8000">localhost:8000</a></code></p>

<h3 dir="auto">Para 'pintar un flujo' con Flow Attack Library </h3>
<p dir="auto">Generar en MITRE Navigator la imagen SVG de las tácticas empleadas y guardarlo en <code>attack-flow/images</code><br>
Generar un flujo de ataque (.json) y guardarlo en la carpeta <code>attack/corpus</code>:<br>
(las carpetas señaladas solo son una propuesta)</p>
<p dir="auto">Arrancar Poetry <br>
<code>cd attack-flow</code><br>
<code>poetry shell</code></p>

<p dir="auto">'pintar': <code>af matrix images/fichero-entrada.svg corpus/fichero.json fichero-salida.svg</code></p>

