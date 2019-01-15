# pathUbuntu18.04

En este repositorio en enseñare los comandos que tenemos utilizar en Ubuntu 18.04

Más instalar ubuntu debemos que instalar las actualizaciones con el comando en la terminal:

```
sudo apt update && sudo apt upgrade -y
```

Para abrir la terminal en Ubuntu se puede abrir con la combinaciones de tecla `Ctrl` + `Alt`+ `T`. 

### Instalación paquetes:

```
sudo apt install nombre_paquet -y
```

### Instalar varios paquetes a la vez 

Para instalar varios paquetes a la vez dejando un espacio en blanco entre ellos.

```
 sudo  apt install nombre_paquetes nombre_paquete -y 
```

### Desinstalar paquetes:

```
sudo apt remove nombre_paquete
```

### Desinstalar paquetes(incluyendo archivos de configuración):

```
sudo apt remove --purge nombre_paquete
```

## Paquetes con extensión .deb

Otra forma de instalar aplicaciones en el sistema es por medio de los paquetes ya preparados para ser instalados y con extensión .deb.

Para instalr estos paquete sólo tienes que hacer doble click sobre el fichero en el nevegador `Nautilus` y automáticamente se lanzará el "Centro de Sofware" o la aplicación gdebi(si la tenemos instalada),  que se ocupará de instalar el paquete y buscar las dependencias de otros paquetes que pudiera necesitar para correcta instalación.

Si lo preferimos, también se pueden instalar mediante la línea de comandos, mediante el comando dpkg:

```
sudo dpkg -i nombre_paquete.deb
```

El mismo comando también se puede usar para desinstalar el paquete .deb:

```
sudo dpkg -r nombre_paquete.deb
```
