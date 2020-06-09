# TúTubo
 
A minimal Youtube project


## Contribución

Para clonar este repositorio junto a todos los otros del proyecto, se debe correr:

	git clone --recursive git@github.com:NachoRaik/tutubo.git

Consideraciones: 

- Los subrepos estarán apuntando a algún commit en particular, recordar hacer `checkout` y `pull` de lo último a la hora de trabajar sobre ellos.
- El clone se hará mediante SSH, por lo que deberá configurarla, de no tenerla.
- Para versiones anteriores de Git, es posible que deba hacerse además: `git submodule update --init --recursive` 


## Levantar todo el sistema local

Para levantar local el sistema, se debe correr el siguiente comando:

	docker-compose up --build

Para pegarle a cada servicio:
- AppServer --> http://localhost:5000
- AuthServer --> http://localhost:3000
- MediaServer --> http://localhost:5005

**Disclaimer:** Para probar el flujo de la app, se le debería pegar únicamente al AppServer
