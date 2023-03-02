*** MITRE ASSISTANT *************
comprobar que se ejecuta y ayuda
$ mitre-assistant -h

Ejemplos de Querys
mitre-assistant search -m enterprise -t "fin4,fin5,fin6,fin7"
mitre-assistant search -m enterprise -t "APT18,APT19,Aquatic-Panda"
mitre-assistant search -m enterprise -t "persistence"
mitre-assistant search -m enterprise -t "mimikatz"
mitre-assistant search -m enterprise -t "stats:datasources" -e csv -f Descargas/DataSources_file.csv

*** MITRE NAVIGATOR ***************
docker start navigator
http:localhost:80


*** Mitre DeTT&CT *****************
cd DeTTECT
python3 dettect.py e
http://localhost:8080

Data sources: cargar ejemplo
Obtener .json
cd DeTTECT
python3 dettect.py ds -fd input/DS_Rooted.yaml -l


*** FLOW ATT&CK *******************
docker start AttackFlowBuilder
http://localhost:8000/

Pintar el flujo
cd attack-flow
poetry shell
af matrix rooted/ContiPWCFlow.svg rooted/Conti_PWC.json rooted/ContiPWC-secuencia.svg


*** CALDERA **************
cd caldera
python3 server.py --insecure
http://localhost:8888



