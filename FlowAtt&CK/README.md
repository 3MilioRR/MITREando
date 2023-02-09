FLOW ATT&CK

Ejecutar la aplicación on-line (online builder)
https://center-for-threat-informed-defense.github.io/attack-flow/ui/

Ejecutar la aplicación en la máquina virtual
docker start AttackFlowBuilder
localhost:8000
   
Ejecutar Attack Flow Library (solo en la máquin a virtual)
cd attack-flow
poetry shell

Para 'pintar un flujo' (las carpetas solo son una propuesta)
Generar en MITRE Navigator la imagen SVG de las tácticas empleadas y guardarlo en attack-flow/imnages
Generar un flujo de ataque (.josn) y guardarlo en la carpeta attack/corpus
$ af matrix images/fichero-entrada.svg corpus/fichero.json fichero-salida.svg
