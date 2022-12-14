Back-end de WSL 2馃敆

Windows 11 de 64 bits: Home o Pro versi贸n 21H2 o superior, o Enterprise o Education versi贸n 21H2 o superior.
Windows 10 de 64 bits: Home o Pro 21H1 (compilaci贸n 19043) o superior, o Enterprise o Education 20H2 (compilaci贸n 19042) o superior.
Habilite la funci贸n WSL 2 en Windows. Para obtener instrucciones detalladas, consulte la documentaci贸n de Microsoft.
Se requieren los siguientes requisitos previos de hardware para ejecutar correctamente WSL 2 en Windows 10 o Windows 11:

Procesador de 64 bits con traducci贸n de direcciones de segundo nivel (SLAT)
RAM del sistema de 4GB
El soporte de virtualizaci贸n de hardware a nivel de BIOS debe estar habilitado en la configuraci贸n del BIOS. Para obtener m谩s informaci贸n, consulte Virtualizaci贸n.
Descargue e instale el paquete de actualizaci贸n del kernel de Linux.

Los contenedores y las im谩genes creadas con Docker Desktop se comparten entre todas las cuentas de usuario en las m谩quinas donde est谩 instalado. Esto se debe a que todas las cuentas de Windows usan la misma m谩quina virtual para crear y ejecutar contenedores. Tenga en cuenta que no es posible compartir contenedores e im谩genes entre cuentas de usuario cuando se usa el backend Docker Desktop WSL 2.

La ejecuci贸n de Docker Desktop dentro de un VMware ESXi o Azure VM es compatible con los clientes de Docker Business. Primero requiere habilitar la virtualizaci贸n anidada en el hipervisor. Para obtener m谩s informaci贸n, consulte Ejecuci贸n de Docker Desktop en un entorno de VM o VDI.

Instalar Docker Desktop en Windows
Instalar de forma interactiva
Haga doble clic en Docker Desktop Installer.exe para ejecutar el instalador.

Si a煤n no ha descargado el instalador (Docker Desktop Installer.exe), puede obtenerlo de Docker Hub. Por lo general, se descarga en la carpeta Descargas, o puede ejecutarlo desde la barra de descargas recientes en la parte inferior de su navegador web.

Cuando se le solicite, aseg煤rese de que la opci贸n Usar WSL 2 en lugar de Hyper-V en la p谩gina Configuraci贸n est茅 seleccionada o no, seg煤n su elecci贸n de back-end.

Si su sistema solo admite una de las dos opciones, no podr谩 seleccionar qu茅 backend usar.

Siga las instrucciones del asistente de instalaci贸n para autorizar al instalador y continuar con la instalaci贸n.

Cuando la instalaci贸n sea exitosa, haga clic en Cerrar para completar el proceso de instalaci贸n.

Si su cuenta de administrador es diferente a su cuenta de usuario, debe agregar el usuario al grupo de usuarios de docker. Ejecute Administraci贸n de equipos como administrador y vaya a Usuarios y grupos locales > Grupos > usuarios de docker. Haga clic derecho para agregar el usuario al grupo. Cierre sesi贸n y vuelva a iniciarla para que los cambios surtan efecto.