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

## Key cloack
http://localhost:8080/auth/realms/localRealm/.well-known/openid-configuration


### Kibana Setup

```bash
docker-compose -f docker-compose-filebeat.yml build
docker-compose -f docker-compose-filebeat.yml run filebeat filebeat setup
```

```bash
docker-compose -f docker-compose-filebeat-apache.yml build
docker-compose -f docker-compose-filebeat-apache.yml up
```

### Ingest nginx log
```bash
docker-compose -f docker-compose-filebeat.yml up
```

### Elastic clean

## Curator 
Projet docker à builder: 
https://github.com/elastic/curator


## Error page
* destroy people : https://threejs.org/examples/#webgl_points_dynamic
* o en lave : https://threejs.org/examples/#webgl_shader_lava
* annimeau fuite: https://threejs.org/examples/#webgl_shadowmap
* OCTOTERMINATOR: https://threejs.org/examples/#webgl_loader_assimp
* destroy : https://threejs.org/examples/#webgl_physics_convex_break
* molecule: https://threejs.org/examples/#css3d_molecules
* cube: https://shaunlebron.github.io/cube/
* yeu vous suive: https://codepen.io/hakimel/pen/vfykn
* texte no vacancy: https://codepen.io/rileyjshaw/pen/ufEIH
* Lampe dans le noir: https://codepen.io/davedehaan/pen/DHjIC
* texte erreur: https://codepen.io/ZonFire99/pen/njdls
 

