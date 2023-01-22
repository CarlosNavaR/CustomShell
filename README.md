
# Descripción 🚀

Este repositorio es creado con la intención de tener una guía para replicar la customization de mi terminar actual *Git bash* puede ser aplicada a cualquier otra terminal del entorno windows (Leer documentación).

`Buz 👩‍🚀`

# Requisitos

[X] [Git](https://git-scm.com/downloads)
[X] [VsCode](https://code.visualstudio.com/)

# Enlaces importante ⚠

[X] [OhMyPosh](https://ohmyposh.dev/docs/)
[X] [NerdFonts](https://www.nerdfonts.com/)

# Instalación 💾
Existen diversas formas de instalar esta herramienta, el flujo que se siguió es por medio de la terminal (powershell).

1. Instalar OhMyBash [ [Windows](https://ohmyposh.dev/docs/installation/windows) ]
```sh
  winget install JanDeDobbeleer.OhMyPosh -s winget
```

Este comando permite la instalación de algunas dependencias necesarias
- oh-my-posh.exe - Ejecutable Windows
- themes - Los temas mas recientes

2. Instala fuente dentro del sistema [ [NerdFonts](https://www.nerdfonts.com/) ]
NerdFonts es un banco de fuentes de tipografía que proporciona símbolos e iconos adicionales para mostrar contenido gráfico dentro de la terminal. 

`Fuente recomendada` [FiraCode](https://github.com/ryanoasis/nerd-fonts/releases/download/v2.3.0/FiraCode.zip)

2.1 - Configurar fuente en visual studio code
Dentro de la configuración `ctrl + ,` abrir la configuración en archivo json, después solo queda copiar y pegar la siguiente linea, en caso de instalar una fuente que no sea FiraCode sera requerido ver el nombre y reemplazarla.

```sh
  "terminal.integrated.fontFamily": "FiraCode Nerd Font",
```

3.- Configuración de la terminal
Una vez dentro de la termina que se requiera configurar en este caso `Git Bash` se ejecutara el siguiente comando el cual debería de retornar `bash`.

```sh
  oh-my-posh get shell
```

Una vez estamos seguros que la terminal es bash es requerido ir a la ruta raíz de nuestro usuario `C:\Users\Username` en este usuario crearemos un archivo con el nombre de `.bashrc` es importante verificar que no se guarde como archivo de txt, recomendable abrir en vs code para verificar el tipo de archivo. En caso de no tener una terminal bash verificar el método de instalación seguir la documentación [otras terminales](https://ohmyposh.dev/docs/installation/prompt).

Cuando ya se tenga el archivo `.bashrc` creado solo es necesario pegar el siguiente texto.

```sh 
  eval "$(oh-my-posh init bash)"
```

Ahora solo queda ejecutar el siguiente comando 

```sh 
  exec bash
```

La interfaz de la terminal se actualizara y posiblemente se mostraran caracteres especiales.

<center> 

![Terminal con caracteres especiales](/images/FirstConsole.PNG "Ejemplo de terminal").

</center>


Para solucionar este problema solo es requerido dar click derecho sobre el nombre de la venta y abrir propiedades -> Text, en el apartado de texto seleccionar la fuente que elegimos para nuestra terminal, una vez se elige la Nerd Font de nuestra preferencia se corregirá automáticamente.

Una vez realizado todo esto tendremos lista nuestra terminal personalizada, ahora es cuestión de que tan personalizada queremos nuestra terminal, ya que se puede realizar configuración manualmente u optar por un tema ya definido [Temas](https://ohmyposh.dev/docs/themes).


`Buz 👩‍🚀`

