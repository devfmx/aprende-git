# Instala y configura Git

El proceso de instalación varía un poco según el sistema operativo de tu computadora.

## Instalación en Windows

Para Windows, es recomendable descargarlo desde [git for windows](https://gitforwindows.org/). Este sitio ofrece en la descarga, además de Git, un conjunto de herramientas ligeras de gran utilidad en Windows, como una [terminal que emula los comandos de UNIX](https://www.atlassian.com/es/git/tutorials/git-bash) (_estos son los comandos empleados en macOs y Linux_).

## Instalación en MacOS y Linux

Para **macOs** y **Linux/Unix** puedes descargar git directamente del [sitio web oficial](https://git-scm.com/downloads).

## Comprueba tu instalación

Una vez instalado Git, puedes probar si la instalación fue exitosa abriendo una terminal (_busca una aplicación llamada terminal o [iTerm](https://iterm2.com/) en macOs, terminal en Linux, y git bash en Windows_).

Sobre la terminal escribe `git --version` y presiona `Enter`.

Enseguida debe aparecer un número, que refleja la versión de git instalada en tu sistema.

## ¿Cómo utilizo Git?

Su uso principal es mediante la ejecución de comandos en una terminal, a través de una [interfaz de línea de comandos](https://es.wikipedia.org/wiki/Interfaz_de_l%C3%ADnea_de_comandos) (_CLI por sus siglas en inglés_).

Cuando ejecutaste `git --version`, comprobaste que la CLI fue instalada exitosamente, y que puedes ejecutar comandos de git.

Para utilizar git se emplea la terminal. Escribimos la palabra _git_ seguida de instrucciones específicas que queremos realizar, como guardar un cambio, o visualizar las últimas modificaciones.

![Terminal de computadora ejecutando comandos de Git](https://storage.googleapis.com/campus-cvs/guia-code/git-terminal-2.png)

Prueba escribiendo y ejecutando el siguiente comando `git status` en tu terminal y observa qué sucede:

```javascript
git config
```


## Configuración inicial

Desde la terminal, se puede acceder a la guía de comandos de configuración con el comando:

```javascript
git config
```

Ahora vamos a establecer una identidad en Git, para vincular tus cambios y contribuciones a tu cuenta de Github al momento de hacer _commits_. Para ello usamos los comandos:

```javascript
git config user.name
git config user.email
```

Al ejecutar estos comandos, nos muestra qué valores tiene almacenados Git de nombre de usuario y correo electrónico en nuestra computadora.

- Si no te muestra nada, no te preocupes, es normal al usar git por primera vez.

- Si te muestra algo, quiere decir que **ya has configurado previamente estos valores** y no es obligatorio realizar el siguiente paso.

Para establecer nuestro nombre de usuario y correo, empleamos los siguientes comandos:

```javascript
git config --global user.name "devf"
git config --global user.email "german@devf.mx"
```

Finalmente, prueba ejecutando nuevamente los comandos, y observarás los valores que acabas de ingresar para nombre de usuario y correo:

```javascript
git config user.name
git config user.email
```

También puedes probar listando todos los valores de configuracion con:

```javascript
git config --list
```
