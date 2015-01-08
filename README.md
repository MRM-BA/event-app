# EventApp

Aplicación para publicar fotos automáticamente en distintos eventos de Facebook.

Es el primer intento de crear una aplicación mobile por parte del equipo de front-end de MRM.

## Requisitos

- [Node.js](http://nodejs.org/)
- [EditorConfig](http://editorconfig.org/) (si el editor de texto que utilizas tiene soporte de este plugin)

## Instalación de las herramientas

Pasos para la instalación de todas las herramientas necesarias para comenzar a desarrollar:
1. Instalar los SDK de los dispositivos para los que vayamos a desarrollar. Para este proyecto utilizaremos Android. Para lograrlo, hay que seguir estos pasos:
  1. Comprobar si cumple con los requisitos de sistema: [http://developer.android.com/sdk/index.html#Requirements](http://developer.android.com/sdk/index.html#Requirements)
  2. Descargar e instalar JDK desde [http://www.oracle.com/technetwork/java/javase/downloads/index.html](http://www.oracle.com/technetwork/java/javase/downloads/index.html) y reiniciar la máquina al finalizar.
  3. Crear la variable de entorno "JAVA_HOME" y cargarla con la ruta al JDK (por ejemplo, C:\Program Files\Java\jdk1.8.0_11). Agregar a la variable path la ruta de la carpeta "bin" de JAVA, que es "%JAVA_HOME%\bin".
  4. Descargar Apache Ant para poder realizar las compilaciones de Android. Descargar el zip desde [http://ant.apache.org/bindownload.cgi](http://ant.apache.org/bindownload.cgi) y luego descomprimirlo dentro de la unidad C.
  5. Crear la variable de entorno "ANT_HOME" y cargarla con la ruta a la carpeta donde se descomprimió Apache Ant (por ejemplo, C:\Program Files\Java\jdk1.8.0_11). Agregar a la variable path la ruta de la carpeta "bin" de ANT, que es "%ANT_HOME%\bin".
  6. Descargar e instalar Android Studio desde [http://developer.android.com/sdk/index.html](http://developer.android.com/sdk/index.html). Se recomienda instalar el SDK en la carpeta de usuario para no tener problemas con los permisos de administrador al instalar paquetes o actualizaciones.
  7. Cargar en la variable de entorno "PATH" la ruta a las carpetas "platform-tools" y "tools" del SDK de Android. __NOTA:__ se recomienda cargar la ruta absoluta, sin utilizar otra variable de entorno en el ruteo.
  8. Ingresar al Android SDK Manager y comprobar que estén instaladas los paquetes "Intel x86 Atom System Image", "Intel x86 Atom_64 System Image" y "Extra/Intel x86 Emulator Accelerator (HAXM Installer)". Si no lo están, instalarlos. Lo mismo para "Android 4.4.2 (API 19)".
  9. Si al correr un device lanza error, ejecutar manualmente el archivo "{CARPETA SDK}\extras\intel\Hardware_Accelerated_Execution_Manager\intelhaxm-android.exe". Si la instalación lanza un error del tipo **VT not supported** ejecutar este comando
  ```
  dism.exe /Online /Disable-Feature:Microsoft-Hyper-V
  ```
  y, en caso de tener un microprocesador Intel, habilitar en la BIOS, en la sección ADVANCED, tanto **Intel Virtualization Technology (VTx)** como **Virtualization Technology for Directed I/O (VT-d)**
2. Instalar Apache Cordova CLI globalmente a través de la consola de comandos. Para eso, ejecutar:
```
npm install -g cordova
```
