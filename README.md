# Entrega TPFinal Grupo 8 - Computacion Aplicada

## 1. Armando el equipo

[x] La contraseña de root fue blanqueada y cambiada a la pedida

[x] Nombre de la maquina virtual establecida como TPServer

## 2. Servicios

[x] Instalado SSH > openssh

[x] Pemite loguear con clave publica de Blackboard, (la carpeta .ssh se encuentra en /home/)

[x] Instalado Apache > apache2

[x] Instalado PHP7.3

[x] Arreglado error sintaxis en index.php

[x] Subido a /var/www/html

[x] Instalado MYSQL > mariadb

[x] Arreglado error de sintaxis en db.sql

[x] db.sql cargado a MYSQL

[x] LAMP stack corriendo en la red local, index.php conecta correctamente a la base de datos y levanta la query.

-- NOTA: Se instalo SAMBA para permitir el facil intercambio archivos entre la maquina anfitriona y la maquina virtual

## 3. Storage

[x] Agregado disco nuevo de 10GB con 2 particiones estandar (83 en la tabla de particiones)

[x] Montada particion 1 en /www_dir 3GB

[x] Montada particion 2 en /backup_dir 6GB

[x] Creado symlink de /var/www/html/index.php en /www_dir

[x] Cambiado DOCUMENT_ROOT en apache2

[x] fstab configurado para que ambos directorios se monten al inicio del sistema

## 4. Redes

[x] Creada placa de red nueva del tipo "Host-only Adapter"

[x] Configurada interface enp0s0 para tener un ip estatica 192.168.56.120, una Mascara de red 255.255.255.0 y Gateway 192.168.56.1 y arrancar automaticamente en archivo /etc/network/interfaces 

-- NOTA: "Host-only Adapter" fue la unica opcion en la que funcionaron los cambios

## 5. Backup

[x] Script backup_full.sh creado en /opt/scripts

[x] Configurada tarea cron (crontab -e) para que haga backup de /var/logs todos los dias a las 0hs

[x] Configurada tarea cron para que haga backup de /www_dir los Lunes, Miercoles y Viernes a las 23hs

[x] Nombres de archivos con formato  [archivos]\_bkp\_[YYYMMDD].tar.gz

[x] Archivos de backup se guardan en /backup_dir

[x] Script valida que los filesystem origen y destino existan previo a su ejecucion.

[x] Origen y destino se pasan como argumentos del script

[x] Script posee opcion -h de ayuda

[x] Script agregado al cron

## 6. Entregables 

[x] Directorio /root, /etc/, /opt/, /www_dir y /backup_dir comprimido en formato .tar.gz

[x] Directorio /var particionado en partes de 20MB

[x] Diagrama topologico de la infraestructura armada
