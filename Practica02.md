_Manos a la obra, Docker a full ..._
_Antes que nada si queremos comprobar si tenemos un contenedor ya instalado o activo lo podemos hacer mediante el siguiente comando 
(de antemano no hay ninguna imagen o contenedor disponible)_

## Muestra los contenedores activos
```
$ docker ps
```

## Contenedores activos y muertos + primeros 10
```
$ docker ps -a | head 
```

_ahora que ya sbemos como se listan los contenedores y como resultado obtuvimos solamente unas cabeceras vacias vamos a instalar nuestras primeras imagenes_

## Instalar un contenedor del tipo alpine, al no especificar la versión de la imagen nos descargará la más actual
```
$ docker pull alpine
```

## Instalar un contenedor del tipo alpine con versión especifica, esto sirve cuando tenemos una aplicacón o necesidad muy especifica
```
$ docker pull alpine:3.7
```

## El comando run nos sirve para arrancar o ejecutar un contenedor, en este caso lo haremos con un contenemos del tipo alpine con versión especifica
```
$ docker run alpine:3.7 ls -l
```

## Si queremos entrar a un contenedor especifico y ejecutar una terminal de manera interactiva lo hacemos con el siguiente comando
```
$ docker run -it alpine:3.7 sh
```
