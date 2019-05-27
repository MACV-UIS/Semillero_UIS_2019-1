# Semillero UIS 2019-1

<img src="Semillero_2019-I/imgs/Banner_Logo.jpeg" style="width:400px;">

##Instrucciones de configuración
Para poder ejecutar experimentos desde casa es necesario instalar VirtualBox, su pack de extensiones y utilidades. Finalmente montar la máquina virtual.

- VirtualBox puede descargarse desde su sitio oficial [aquí](https://www.virtualbox.org/wiki/Downloads)  (Seleccionar Windows Hosts o Linux Hosts en función de el sistema operativo que tenga tu máquina local).

- virtualbox extension pack puede descargarse desde su sitio oficial [aquí](https://download.virtualbox.org/virtualbox/6.0.8/Oracle_VM_VirtualBox_Extension_Pack-6.0.8.vbox-extpack), para instalarlo se debe tener previamente instalado VirtualBox.

- La máquina virtual puede descargarse [aquí](https://drive.google.com/file/d/1KxCUZlXDgyvJzfs6s7EfegMVS1HL_bXq/view?usp=sharing)



# Máquina Virtual

## Montando la máquina virtual:

- Abrimos VirtualBox

- Seleccionamos Archivo/Importar servicio virtualizado

- Damos click sobre la carpeta y buscaremos el directorio donde descargamos nuestra máquina virtual (archivo.ova)

Usaremos esta máquina virtual que tiene instalado un entorno Python Anaconda con Jupyter Notebooks disponibles en  [localhost:8008/tree](http://localhost:8008/tree) una vez que la máquina arranca.

**Observa la configuración de la máquina**

- Si tu máquina física tiene al menos 4GB de memoria configura la máquina virtual **con 2GB de memoria** (se recomienda utilizar máximo el 50% de la memoria disponible)
- Aunque casi no necesitarás un terminal, el interfaz de Jupyter Notebooks tiene un terminal para acceder a través del navegador. En cualquier caso, la máquina virtual tiene un servidor SSH en el puerto 2222 con user/user como usuario y pwd. Si tu máquina física es mac o linux usa `ssh -p 2222 user@localhost` para conectarte. Si es windows, usa [putty](https://www.putty.org/)
- Si compartes una carpeta entre la física y virtual asegúrate que **el nombre cone el que se comparte** sea `share` (aunque el nombre de la carpeta en la máquina física puede ser distinto)

recuerda que debes tener carpetas compartidas, para ello verifica que existan registros en: 
    - Click derecho sobre la máquina virtual
    - Configuración
    - Carpetas Compartidas
    - En caso de que no existan registros, agregar una carpeta compartida.

**Para montar la carpeta compartida** ejecuta lo siguiente en un terminal y la carpeta aparecerá en /home/user/share:

    sudo mount share

    
## Descargar Repositorio desde casa
para descargar nuestro repositorio desde casa realizaremos los siguientes pasos:

- Abrimos Jupyter Notebook [localhost:8008/tree](http://localhost:8008/tree) una vez que la máquina arranca.
- Abrimos un terminal  (damos click sobre new / terminal).
- En la consola escribimos cd CarpetaCompartida (por defecto, cd share)
- finalmente ejecutamos el comando: git clone https://github.com/MACV-UIS/Semillero_UIS_2019-1.git








