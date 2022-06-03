# Azure comunicación entre dos VM por medio de redes virtuales

Se van a crear dos redes virtuals en Azure, posteriormente se van a crear dos VM en Azure, asignando una red virtual a cada una para finalmente comunicar ambas redes virtuales entre sí y así lograr comunicación entre las VM también.

![Logo de VM](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/VM.jpg)

## Requisitos

- Cuenta de [Azure](https://portal.azure.com/) con suscripción activa
- Computadora con Windows, Linux o MacOs

---------------------------------------------------------

## Pasos

- Se inicia sesión en la página de [Azure](https://portal.azure.com/)

![P5-0](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/inicio%20Azure.PNG)

- Se busca "Máquinas virtuales" y se presiona enter

![P5-1](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-1.PNG)

- Se selecciona "crear" en la esquina superior izquierda y después "Máquina virtual de Azure"

![P5-2](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-2.PNG)

- En el apartado de grupo de recursos se da click en "crear nuevo", se coloca un nombre y se da click en "aceptar"

![P5-3](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-3.PNG)

- Se coloca un nombre para la máquina virtual, se selecciona una región (autralia recomendada por disponibilidad y precio) y se selcciona windows como sistema operativo

![P5-4](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-4.PNG)

- Más abajo se coloca un nombre de usuario y se crea una contraseña para ese usuario (importante recordar el nombre de usuario y contraseña)

![P5-5](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-5.PNG)

- Más abajo se marca la opción de licencia válida de Windows y se presiona el botón "revisar y crear"

![P5-6](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-6.PNG)

- Se abrirá otra ventana donde debemos esperar a que se habiite la opción de crear, cuando se habilite la presionamos

![P5-7](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-7.PNG)

- Mostrará una ventan donde indica que el recurso esta siendo creado

![P5-8](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-8.PNG)

- Una vez terminada la implementación se mostrará una ventana como la siguiente:

![P5-9](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-9.PNG)

- Ahora se procede a crear otra máquina virtual

- Se inicia sesión en la página de [Azure](https://portal.azure.com/)

![P5-0](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/inicio%20Azure.PNG)

- Se busca "Máquinas virtuales" y se presiona enter

![P5-1](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-1.PNG)

- Se selecciona "crear" en la esquina superior izquierda y después "Máquina virtual de Azure"

![P5-2](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-2.PNG)

- En el apartado grupo de recursos se selecciona el mismo que se creó para la otra máquina virtual

![P5-10](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-10.PNG)

- Los demás apartados de más abajo también se llenan, es necesario colocar un nuevo nombre, región (de preferencia la misma que la otra máquina virtual) e imagen (Windows)

![P5-11](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-11.PNG)

- Se crea de igual forma un usuario con su respectiva contraseña (pueden ser los mismoa que los de la otra máquina virtual)

![P5-12](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-12.PNG)

- Más abajo se marca la opción de licencia válida de Windows y se presiona el botón "revisar y crear"

![P5-13](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-13.PNG)

- Se navega hacia arriba sobre la misma pestaña y se busca la parte donde dice "redes" y se da click

![P5-14](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-14.PNG)

- En la nueva ventana se selecciona en la parte de red virtual la red que contenga el nombre del grupo de recursos que creamos

![P5-15](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-15.PNG)

- Se baja más sobre la pestaña y se presiona "revisar y crear"

![P5-16](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-16.PNG)

- En la siguiente pestaña esperamos a que termine la validación y se habilite el botón de "crear". Una vez habilitado se da click en el mismo.

![P5-17](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-17.PNG)

- Se muestra otra ventana donde dice que el recurso está en proceso de implementación. Esperamos

![P5-18](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-18.PNG)

- Ahora vamos al buscador de windows en la parte inferior izquierda de nuestra computadora, buscamos "Windows store" y abrimos el primer resultado

- Nos abrirá la tienda de windows, en el buscador superior buscamos "escritorio remoto de Microsoft" y le damos click al resultado marcado en la imagen

![P5-19](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-19.PNG)

- Le damos click en "obtener" y esperamos a que se instale

![P5-20](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-20.PNG)

- Al terminar de instalarse debe aparecer así

![P5-21](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-21.PNG)

- Volvemos al navegador para corroborar si ya se implementó nuestra segunda máquina virtual. Si ya se implementó debe aparecer así

![P5-22](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-22.PNG)

- Volvemos al inicio de [Azure](https://portal.azure.com/) y damos click sobre la primer máquina virtual que creamos

![P5-23](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-23.PNG)

- Dentro del menú lateral del recurso damos click en "conectar"

![P5-24](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-24.PNG)

- En la parte derecha damos click en el botón "descargar"

![P5-25](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-25.PNG)

- Se nos descargará un archivo a la PC, procedemos a abrir el explorador de archivos y buscamos donde se descargó.

![P5-26](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-26.PNG)

- Le damos doble click y seleccionamos "ejecutar con escritorio remoto"

![P5-27](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-27.PNG)

- Abrirá la aplicación que instalamos desdela tienda y nos pedirá permisos para el accceso aceptamos

![P5-28](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-28.PNG)

- Después nos pedirá nuestro usuario y contraseña. Aquí debemos colocar el usuario y contraseña que creamos para la primer máquina virtual. Le damos en conectar.

![P5-29](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-29.PNG)

- En la siguiente ventana le damos en "conectarse de todos modos"

![P5-30](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-30.PNG)

- Nos abrirá la máquina virtual con el inicio de Windows, aquí minimizamos la aplicación de escritorio remoto.

- Después buscamos en Azure la red virtual que creamos dentro del grupo de recursos y le damos click. Dentro del recurso de red virtual en el menú del lado izquierdo seleccionamos "Dispositivos conectados" y nos mostrará las direcciones IP de las dos Máquinas virtuales que creamos, copaimos la IP de la segunda máquina virtual.

![P5-31](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-31.PNG)

- Volvemos a la aplicación de escritorio remoto, aceptamos las configuraciones iniciales y después buscamos powershell en la máquina virtual y la abrimos como administrador.

![P5-32](https://github.com/AlanAlvaradoR/Azure-Comunicacion-VMs/blob/main/imagenes/P5-32.PNG)

