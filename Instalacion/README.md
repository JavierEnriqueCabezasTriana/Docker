Back-end de WSL 2🔗

Windows 11 de 64 bits: Home o Pro versión 21H2 o superior, o Enterprise o Education versión 21H2 o superior.
Windows 10 de 64 bits: Home o Pro 21H1 (compilación 19043) o superior, o Enterprise o Education 20H2 (compilación 19042) o superior.
Habilite la función WSL 2 en Windows. Para obtener instrucciones detalladas, consulte la documentación de Microsoft.
Se requieren los siguientes requisitos previos de hardware para ejecutar correctamente WSL 2 en Windows 10 o Windows 11:

Procesador de 64 bits con traducción de direcciones de segundo nivel (SLAT)
RAM del sistema de 4GB
El soporte de virtualización de hardware a nivel de BIOS debe estar habilitado en la configuración del BIOS. Para obtener más información, consulte Virtualización.
Descargue e instale el paquete de actualización del kernel de Linux.

Los contenedores y las imágenes creadas con Docker Desktop se comparten entre todas las cuentas de usuario en las máquinas donde está instalado. Esto se debe a que todas las cuentas de Windows usan la misma máquina virtual para crear y ejecutar contenedores. Tenga en cuenta que no es posible compartir contenedores e imágenes entre cuentas de usuario cuando se usa el backend Docker Desktop WSL 2.

La ejecución de Docker Desktop dentro de un VMware ESXi o Azure VM es compatible con los clientes de Docker Business. Primero requiere habilitar la virtualización anidada en el hipervisor. Para obtener más información, consulte Ejecución de Docker Desktop en un entorno de VM o VDI.

Instalar Docker Desktop en Windows
Instalar de forma interactiva
Haga doble clic en Docker Desktop Installer.exe para ejecutar el instalador.

Si aún no ha descargado el instalador (Docker Desktop Installer.exe), puede obtenerlo de Docker Hub. Por lo general, se descarga en la carpeta Descargas, o puede ejecutarlo desde la barra de descargas recientes en la parte inferior de su navegador web.

Cuando se le solicite, asegúrese de que la opción Usar WSL 2 en lugar de Hyper-V en la página Configuración esté seleccionada o no, según su elección de back-end.

Si su sistema solo admite una de las dos opciones, no podrá seleccionar qué backend usar.

Siga las instrucciones del asistente de instalación para autorizar al instalador y continuar con la instalación.

Cuando la instalación sea exitosa, haga clic en Cerrar para completar el proceso de instalación.

Si su cuenta de administrador es diferente a su cuenta de usuario, debe agregar el usuario al grupo de usuarios de docker. Ejecute Administración de equipos como administrador y vaya a Usuarios y grupos locales > Grupos > usuarios de docker. Haga clic derecho para agregar el usuario al grupo. Cierre sesión y vuelva a iniciarla para que los cambios surtan efecto.