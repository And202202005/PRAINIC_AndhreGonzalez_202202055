# Manual de Comandos de Ubuntu

## 1. Navegación entre archivos y directorios

### `cd` - Cambiar de directorio
```sh
cd /ruta/del/directorio
```
Ejemplo:
```sh
cd /home/usuario/Documentos
```

### `pwd` - Mostrar la ruta del directorio actual
```sh
pwd
```

### `ls` - Listar contenido de un directorio
```sh
ls
ls -l   # Muestra detalles de archivos
ls -a   # Muestra archivos ocultos
ls -la  # Muestra todos los archivos con detalles
```

## 2. Ver contenido de un directorio
```sh
ls
ls -lh  # Muestra tamaños en formato legible
ls -lt  # Ordena por fecha de modificación
```

## 3. Crear carpetas en un directorio
### `mkdir` - Crear un directorio
```sh
mkdir nombre_directorio
```
Ejemplo:
```sh
mkdir Proyectos
```

### Crear múltiples directorios a la vez
```sh
mkdir dir1 dir2 dir3
```

## 4. Copiar archivos y carpetas
### `cp` - Copiar archivos
```sh
cp archivo_origen archivo_destino
```
Ejemplo:
```sh
cp documento.txt /home/usuario/Documentos/
```

### Copiar directorios
```sh
cp -r directorio_origen directorio_destino
```
Ejemplo:
```sh
cp -r Proyecto/ /home/usuario/Respaldo/
```

## 5. Mover archivos y carpetas
### `mv` - Mover o renombrar archivos
```sh
mv archivo_origen archivo_destino
```
Ejemplo:
```sh
mv viejo_nombre.txt nuevo_nombre.txt
mv archivo.txt /home/usuario/Descargas/
```

## 6. Eliminar archivos y carpetas
### `rm` - Eliminar archivos
```sh
rm archivo.txt
```

### `rm -r` - Eliminar carpetas
```sh
rm -r directorio
```

## 7. Ingresar como superusuario
### `sudo` - Ejecutar comandos como superusuario
```sh
sudo comando
```
Ejemplo:
```sh
sudo apt update
```

### `su` - Cambiar a usuario root
```sh
su
```

## 8. Modificar permisos
### `chmod` - Cambiar permisos de archivos
```sh
chmod 755 archivo
```
Ejemplo:
```sh
chmod +x script.sh
```

## 9. Crear/editar archivos de texto desde la terminal
### `nano` - Editor de texto en terminal
```sh
nano archivo.txt
```

### `touch` - Crear un archivo vacío
```sh
touch archivo.txt
```

## 10. Instalar paquetes
### `apt install` - Instalar paquetes con APT
```sh
sudo apt install nombre_paquete
```
Ejemplo:
```sh
sudo apt install vim
```

## 11. Actualizar paquetes
### `apt update` y `apt upgrade`
```sh
sudo apt update  # Actualiza lista de paquetes
sudo apt upgrade # Instala actualizaciones
```

## 12. Eliminar paquetes
### `apt remove` - Desinstalar paquetes
```sh
sudo apt remove nombre_paquete
```
Ejemplo:
```sh
sudo apt remove vim
