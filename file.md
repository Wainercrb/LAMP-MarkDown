# Configuración de una servidor LAMP
1.  Actualización de la maquina
```cmd
    sudo apt-get update
```
2. Instalar apache
```cmd
    sudo apt-get install apache2
``` 

3. Abrir el navergador firefox y entral a localhost para verificar si apache realemte esta instalado, si apareche un pagin de apache se instalo correctamente.
4. Instalación de Mysql
```CMD
    sudo apt-get install mysql-client -mysql-ser php-mysql
```
5. para verificar que mysql esta instaldo escribe
```CMD
    systemctl status mysql.service
```
6. instalmos php
```CMD
    sudo apt-get install php -y
``` 
7. Para comprobar que php se instalo haremos los siguines pasos

* vamos al homd de apache
```CMD
  cd /var/www/html
```
* Con eliminamos ese archivo index.html
 ```CMD
    sudo rm index.html
 ```
* Creamos un nuevo index.php 
```CMD
    sudo nano index.php
```
* Para verifica que ese php se instar escrimimos en el shell

```PHP
    <?php 
        phpinfo();
    <?

```
* Tiene que apareche un cuadro con la información php
8. Subimos la pagina deseado el servidor por medio del hell, en mi caso era un archivo comprimido que estaba en descargas, entonces la linea de comandos es la siguiente. El home url del servidor es var/www/html
```CMD
    sudo cp filnename.zip /var/www/html
```
9. Eliminamos el index.php que habia con 
```CMD
    sudo rm index.php
```
10. Desconprimimos el zip
```CMD
    unzip filename.zip
```
11. Represcamos el navegador
***
### Credo por Waine Rodriguez Bonilla | UTN








 