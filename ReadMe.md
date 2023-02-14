# Docker + Python

---
# Creamos un contenedor sencillo con Python

```$ docker run -it --rm -v "$PWD":/usr/src/myapp -w /usr/src/myapp python:3 python script.py```

`docker` es el comando base, el daemon

`run` para crear el contenedor

`-it` dos opciones que me valen para interactuar con la terminal del contenedor

`--rm` borra el contenedor cuando finaliza la acción

`-v` define el mapeo del volumen a continuacón

- `PWD` el directorio donde estamos
- `/user/src/myapp` el directorio dentro del contenedor

`-w` es el directorio de trabajo (_workdir_)

`python:3` imagen de la que se creará el contenedor

`python script.py` es el comando para ejecutar dentro del contenedor