<H1># Instrucciones para ejecutar MITRE Assistant</H1>

<p>Antes de nada, comprobar que funciona:<br>
<code>mitre-assistant -h</code></p>

<p><strong>Paso 1 - </strong> Descargar (actualizar) los datos de la matriz de Mitre ATT&CK Empresarial.<br>
<code>mitre-assistant download -m enterprise</code></p>

<p><strong>Paso 2 - </strong> Parsear los datos para poder tratarlos con el programa. <br>
<code>mitre-assistant baseline -m enterprise</code></p>

<h3>Ejecutar Mitre Assistant</h3>
<p>Ejemplos de Querys<br>
<code>mitre-assistant search -m enterprise -t "fin4,fin5,fin6,fin7,fin8"</code><br>
<code>mitre-assistant search -m enterprise -t "persistence"</code><br>
<code>mitre-assistant search -m enterprise -t "mimikatz"</code><br>
<code>mitre-assistant search -m enterprise -t "stats:datasources"-e csv -f DataSources_file.csv</code></p>
