# Cómo descargar repositorios

Uno de los principales propósitos de Github, es permitir **clonar** o descargar un repositorio a tu computadora.

Se le llama **clonar** porque estamos generando una copia exacta del repositorio, y tendremos total libertad de manipular el código localmente, sin afectar el código que obtuvimos desde Github.

![Copias idénticas](https://storage.googleapis.com/campus-cvs/guia-code/git-clone.jpg)

## ¿Cómo clonar un repositorio?

Prueba ingresando al [siguiente repositorio](https://github.com/getify/You-Dont-Know-JS). Este es el repositorio del libro [You Don't Know JavaScript](https://www.amazon.com/You-Dont-Know-Js-Book/dp/B01AY9P0P6), escrito por Kyle Simpson.

Todo repositorio tiene en su página principal un enorme botón verde del lado derecho.

![Página principal de un repositorio](https://storage.googleapis.com/campus-cvs/guia-code/git-repo-clone.png)

Al hacer click sobre este botón verde, se despliega un pequeño menú donde te ofrece tres opciones:

1. Clonar el repositorio, a través de una url dada.
2. Abrir el repositorio con la aplicación de escritorio Github Desktop.
3. Descargar el repositorio en formato `.zip`

Como estamos aprendiendo a trabajar con git desde la terminal, usaremos la opción **1. Clonar**. Asegúrate de tener seleccionada la pestaña con `HTTPS` y copia la url provista, como se muestra en la imagen de abajo.

![Botón para clonar un repositorio](https://storage.googleapis.com/campus-cvs/guia-code/git-repo-clone-btn.png)

## Pasos para clonar desde terminal

Ya que copiamos la url de github, abre una terminal en tu computadora (_busca una aplicación llamada terminal o [iTerm](https://iterm2.com/) en macOs, terminal en Linux, y git bash en Windows_).

#### 1) Aprende comandos básicos de terminal

Aparte de los comandos de Git, que siempre se comienzan escribiendo la palabra _git_ en nuestra terminal, **todo sistema operativo tiene sus propios comandos de terminal** para realizar tareas como movernos entre directorios, crear o borrar archivos, listar el contenido de un directorio, ejecutar aplicaciones, etc.

En estas instrucciones emplearemos [comandos de **Unix**](https://www.vozidea.com/comandos-basicos-de-la-terminal-linux), que son los que emplean los sistemas operativos Linux y macOs en sus terminales.

Para que en **Windows puedas usar los mismos comandos basados en Unix**, es necesario que sigas estas instrucciones desde una terminal de **git bash**, y no desde `PowerShell` o `CMD`.

Al abrir una terminal en cualquier sistema operativo, esta se abre sobre un directorio en particular.

Si queremos ver en qué directorio estamos posicionados desde la terminal, escribimos el comando `pwd` (_print working directory_)

```terminal
pwd
```

Si queremos listar el contenido del directorio actual, escribimos el comando `ls` (_list_). También podemos ejecutar este comando con algunas opciones adicionales como:

```terminal
ls -a
ls -l
ls -la
```

![comando pwd](https://storage.googleapis.com/campus-cvs/guia-code/pwd.jpg)

#### 2) Posiciónate en el directorio donde desees guardar el clon

Imaginemos el siguiente escenario. Al abrir tu terminal, ejecutas el comando `pwd` y descubres que está posicionada en `C:\Users\German\Documentos`, y te gustaría clonar el repositorio en el directorio `C:\Users\German\Escritorio\devf`.

```
.
├── ...
├── Escritorio
│   ├── foto.jpeg
│   └── devf
├── Descargas
│   └── ...
├── Documentos              
│   ├── info.txt
│   ├── Tareas
│   ├── Proyectos 
│   └── ...
└── ...
```

Apoyándonos del arbol de directorios que tienes arriba, observamos que necesitamos salir del directorio `/Documentos`, entrar al directorio `/Escritorio` y finalmente entrar al directorio `Escritorio/devf`.

Para esto necesitamos usar el comando `cd` (_change directory_). En esencia tenemos tres formas de usar el comando para movernos entre directorios.

1. Entrar desde el directorio actual a un sub-directorio:
```terminal
cd /nombre-de-directorio
```

2. Salir del directorio actual, o subir un nivel:
```terminal
cd ..
```

3. Acceder a una ruta exacta. Puedes obtener estas rutas desde el explorador de archivos:
```terminal
cd C:\Users\German\Escritorio\nombre-de-directorio
```

Tomando lo anterior, para resolver el escenario imaginario planetado necesitamos ejecutar los siguientes comandos.

Nota que usamos el comando `pwd` tras cada movimiendo con `cd` para verificar que nos hemos desplazado a otro directorio correcamente.

```
pwd

cd ..

pwd

cd Escritorio

pwd

cd devf

pwd
```

#### 3) Ejecuta el comando para clonar

Finalmente, ya posicionado dentro del directorio deseado donde quieres guardar tu clon del repositorio de github, ejecutamos el comando

```
git clone https://github.com/getify/You-Dont-Know-JS.git
```

![git clone desde la terminal](https://storage.googleapis.com/campus-cvs/guia-code/git-how-to-clone.png)

#### 4) Verifica la descarga del clon

Si el repositorio se clonó correctamente, puedes usar `ls` para listar los directorios y archivos. Debería aparecer el repositorio en esta lista.

Posteriormente puedes ejecutar `cd You-Dont-Know-JS` para posicionarte dentro del repositorio.

Ahora puedes abrir este repositorio de código desde un editor como VS Code y explorar sus entrañas.
