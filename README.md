# kibana

## Installation
https://www.elastic.co/guide/en/x-pack/5.2/installing-xpack.html#xpack-enabling

### Génération des certificats https

```bash
cd config
# generate root certificat
./genCert.sh genCA
# generate server certificat by domain
./genCert.sh -d 127.0.0.1 genCert
./genCert.sh -d localhost genCert
```

### Démarage de l'application
```bash
docker-compose up
```
