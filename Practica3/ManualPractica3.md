# Manual de Instalación en VirtualBox

**Autor: Fernando Andhre Gonzalez Espinoza - 202202055**

## Instalación de VirtualBox
1. Descarga VirtualBox desde [el sitio oficial](https://www.virtualbox.org/).
2. Instala VirtualBox siguiendo las instrucciones del instalador.
3. Abre VirtualBox y crea una nueva máquina virtual.
4. Configura la máquina virtual con la imagen ISO de Ubuntu.
5. Inicia la máquina virtual e instala Ubuntu dentro de VirtualBox.

## Instalación de Ubuntu en VirtualBox
1. Descarga la imagen ISO de Ubuntu desde [el sitio oficial](https://ubuntu.com/download).
2. Abre VirtualBox y crea una nueva máquina virtual.
3. Asigna memoria RAM y espacio en disco adecuado.
4. Selecciona la imagen ISO de Ubuntu en la configuración de la máquina virtual.
5. Inicia la máquina virtual y sigue las instrucciones del instalador de Ubuntu.
6. Completa la instalación y reinicia la máquina virtual.

## Instalación de Apache en Ubuntu
1. Abre la terminal de Ubuntu.
2. Ejecuta el siguiente comando:
   ```bash
   sudo apt update && sudo apt install apache2 -y
   ```
3. Verifica que Apache esté corriendo con:
   ```bash
   systemctl status apache2
   ```
4. Accede a `http://localhost/` en tu navegador para confirmar que Apache está funcionando.

## Creación de un Servidor
1. Asegúrate de tener Apache instalado.
2. Configura el firewall para permitir tráfico HTTP y HTTPS:
   ```bash
   sudo ufw allow 'Apache Full'
   ```
3. Configura un dominio virtual (opcional):
   ```bash
   sudo nano /etc/apache2/sites-available/000-default.conf
   ```
   Modifica el `DocumentRoot` si es necesario.
4. Reinicia Apache:
   ```bash
   sudo systemctl restart apache2
   ```

## Modificación del Index de Apache
1. Accede al directorio raíz de Apache:
   ```bash
   cd /var/www/html/
   ```
2. Edita el archivo `index.html`:
   ```bash
   sudo nano index.html
   ```
3. Reemplaza el contenido con:
   ```html
   <html>
   <head><title>Mi pagina Apache</title></head>
   <body>
       <h1>Fernando Andhre Gonzalez Espinoza - 202202055</h1>
   </body>
   </html>
   ```
4. Guarda el archivo y cierra el editor.
5. Recarga Apache:
   ```bash
   sudo systemctl restart apache2
   ```
6. Visita `http://localhost/` para ver los cambios.

---
**Fin del Manual**
