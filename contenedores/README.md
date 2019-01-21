# ¿Qué es Docker?

Docker es una plataforma para desarrolladores y administradores de sistemas para desarrollar, implementar y ejecutar aplicaciones con contenedores. El uso de contenedores de Linux para implementar aplicaciones se denomina contenedorización. Los contenedores no son nuevos, pero su uso para implementar aplicaciones fácilmente sí lo es. [Fuente](https://docs.docker.com/get-started/)

La contenedorización es cada vez más popular porque los contenedores son:

+ Flexible: Incluso las aplicaciones más complejas se pueden transportar en contenedores.
+ Ligero: los contenedores aprovechan y comparten el núcleo del host.
+ Intercambiable: puede implementar actualizaciones y actualizaciones sobre la marcha.
+ Portátil: puede compilar localmente, implementarlo en la nube y ejecutar en cualquier lugar.
+ Escalable: puede aumentar y distribuir automáticamente réplicas de contenedores.
+ Apilable: puede apilar servicios verticalmente y sobre la marcha.

***

# Instalar Docker

Antes de instalar Docker CE por primera vez en una nueva máquina host, debe configurar el repositorio de Docker. Después, puede instalar y actualizar Docker desde el repositorio. [Fuente](https://docs.docker.com/install/linux/docker-ce/ubuntu/)

1. Actualizar el índice del paquete ```apt```:
```
$ sudo apt-get update
```

2. Instalar paquetes para permitir que ```apt``` use un repositorio sobre HTTPS::
```
$ sudo apt-get install apt-transport-https ca-certificates curl gnupg2 software-properties-common
```

3. Add Docker’s official GPG key:
```
$ sudo apt-key fingerprint 0EBFCD88
```

4. Configurar el repositorio estable:
```
$ sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
```

5. Actualizar el índice del paquete apt e instalar la última versión de Docker CE:
```
$ sudo apt-get update
$ sudo apt-get install docker-ce
```

Para comprobar que se ha instalado correctamente se ejecutará la imagen ```hello-world````:
![hello](https://github.com/xenahort/proyectoCloudComputing/blob/master/img/pruebaDocker.png)
