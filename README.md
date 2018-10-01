# kibana

## Installation

### Hôte configuration

 
### Génération des certificats https

```bash
cd config
# generate root certificat
./genCert.sh genCA
# generate server certificat by domain
./genCert.sh -d web genCert
./genCert.sh -d localhost genCert
```

### Démarage de l'application
```bash
docker-compose up
```


### Kibana Setup

```bash
docker-compose -f docker-compose-filebeat.yml build
docker-compose -f docker-compose-filebeat.yml run filebeat filebeat setup
```

### Ingest nginx log
```bash
docker-compose -f docker-compose-filebeat.yml up
```
