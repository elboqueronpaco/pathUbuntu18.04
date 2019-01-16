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

## Archivos con extensión .bin

Los archivos con extensión .bin son archivos binarios. No contienen un conjunto de programas o librerías como los paquetes, sino que son el programa en sí mismo.

Normalmente se suelen distribuir bajo este sistema programas comerciales, que pueden ser o no gratuitos, pero que normalmente no son libres.

Cuando descargas un fichero de este tipo de internet y lo guardas en tu sistema, no tendrá permiso para ejecutarse. Para dárselos: 

Lo primero que debes hacer, por consiguiente, es dar a ese fichero el premiso para ejecutarse. Para ello pulsa con el botón derecho sobre él y elige la opción Propiedades. En la pestaña Permiso. Activa la castilla "permitir al archivo ejecutarse como un programa" y cierra la ventana.

Ahora que ya has dado permiso al fichero para poder ejecutarlo haz doble click. Al hacerlo debes elejir ejecutar.

Para realizar este operaciòn mediante terminal:

Primero debes dar permisos de ejecutación con el comando:

```
sudo chmod +x nombre_archivo.bin
```

Después instalamos el archivo binario con el siguente comando:

```
sudo ./nombre_archivo.bin
```

## Paquetes con extensión .sh

Los archifos .sh son scripts y para ejecutarlo en el sistema, hacemos doble click sobre ellos y seleccionamos "ejecutar desde terminal" y si alno no funciona ejecutamos en una terminal el comando:

```
bash nombre_paquete.sh
```

### Manera tradional para todos los GNU-Linux:

Abrimos una terminal, nos situamos en la carpeta donde esté el archivo con el siguiente:

```
cd carpeta
```

Le damos permisos con:

```
chmod +x nombre_paquete.sh
```

Y ejecutamos el script con:

```
./nombre_paquete.sh
```

Si necesitamos hacerlo con root, anteponemos "sudo" al comando:

```
sudo ./nombre_paquete.sh
```
## Archivos de extensión .run

Los archivos .run son asistentes, normalmente gráficos, que ayudan a la instalación. Para ejecutarlos basta introducir en el terminal:

```
./archivo.run
```

Normalmente en el caso de que necesite permisos de superusuario(administrador) pedirá la contraseña; de no ser así con ejecutar en el terminal:

```
sudo sh ./archivo.run
```



