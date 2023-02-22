# Instrucciones para ejecutar MITRE Assistant

Comprobar que funciona:
<code>mitre-assistant -h</code>

Step 1 -   Download the ATT&CK Enterprise Matrix
$> <code>mitre-assistant download -m enterprise</code>

Parse the downloaded matrix into a Mitre-Assistant Baseline
$> <code>mitre-assistant baseline -m enterprise</code>

Ejemplos de Querys
<code>mitre-assistant search -m enterprise -t "fin4,fin5,fin6,fin7,fin8"</code>
<code>mitre-assistant search -m enterprise -t "persistence"</code>
<code>mitre-assistant search -m enterprise -t "mimikatz"</code>
<code>mitre-assistant search -m enterprise -t "stats:datasources"-e csv -f DataSources_file.csv</code>