#Instalación Node en Ubuntu 18.04

## Instalación Nodejs v11.x
```
# Using Ubuntu
curl -sL https://deb.nodesource.com/setup_11.x | sudo -E bash -
sudo apt-get install -y nodejs
```

## Node.js v10.x:

```
# Using Ubuntu
curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
sudo apt-get install -y nodejs
```

## Node.js v8.x:
 ```
 curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
sudo apt-get install -y nodejs
```

Instalara node.js atraves de nvm

Se puede instalar nvma atraves de curl o wget

primero instalar curl en ubuntu mediante el comando en la terminal:

```
sudo apt update
sudo apt install curl -y
```
### Uso de curl:

```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.34.0/install.sh | bash
```

### Uso de Wget:

```
wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.34.0/install.sh | bash
```
```
source ~/.profile
```

Podemos verificar rápidamente que NVM ahora esta instalado y funciona correctamente con el siguiente comando:

```
nvm --version
```

Verificar que versiones hay disponibles de Nodejs con el siguiente comando:

```
nvm ls-remote
```

Para instalar la version de node.js que nos interesa usamos el siguiente comando:

```
nvm install v(numero de version)
```
se puede instalar varias versiones de node y la pudemos utilizar con el comando:
```
nvm use numero_de_version
```