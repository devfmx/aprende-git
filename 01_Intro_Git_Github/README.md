# Intro a Git & Github

Para hablar de Git, es necesario hablar rápidamente de la importancia de llevar un historial y control de versiones en nuestros proyectos.

![Git: Version Control System](https://storage.googleapis.com/campus-cvs/guia-code/git-intro-banner.png)

## ¿Qué es Git?

Es un [sistema de control de versiones](https://es.wikipedia.org/wiki/Control_de_versiones) (_VCS por sus siglas en inglés_). Nos facilita guardar respaldos de nuestras carpetas y archivos, otorgando un historial confiable de nuestro trabajo y el trabajo de aquellos que colaboren en el mismo proyecto.

Puedes pensar en Git como un mecanismo que te otorga _[checkpoints](https://www.youtube.com/watch?v=JJR7ER4_jmk)_ donde se guarda todo tu progreso. Si algo terrible ocurre en el futuro, siempre puede regresar a tu último _checkpoint_ sin temor a destruirlo todo.

En el contexto del trabajo en equipo, permite a varias personas colaborar sobre un mismo proyecto sin preocuparse (tanto) por pisarse los pies al alterar, borrar o crear código que no debía integrarse.

Responde a preguntas como:

- ¿Qué cambios se hicieron?
- ¿Quién hizo los cambios?
- ¿Cuándo se hicieron los cambios?
- ¿Por qué fueron requeridos los cambios?

En resumen, usamos Git para crear y mantener **repositorios**.

## ¿Qué es un repositorio?

Un repositorio es un directorio donde se organiza y mantiene información.

En el caso de Git, **el repositorio es el directorio/folder en tu computadora** donde estará la colección de archivos y carpetas que trabajes.

Es decir, tú trabajas en un directorio como de costumbre, agregando, borrando y cambiando archivos como normalmente harías. Este directorio se transforma en un repositorio en el momento en que ejecutas el comando `git init` desde una terminal.

Cuando un directorio se transforma en un repositorio, la única diferencia es que internamente se agrega una carpeta/directorio oculto llamado `.git`. Este archivo es el responsable de manejar las versiones y contener toda la información relacionada a tu proyecto como _commits_, _dirección del repositorio o repositorios remotos_, etc.

#### Repositorio local _versus_ Repositorio remoto

![Repositorio remoto en la nube interactúa con repositorio local](https://storage.googleapis.com/campus-cvs/guia-code/git-repo.png)

Git se trabaja en un **repositorio local**, es decir desde nuestras computadoras, como hacemos usualmente con cualquier directorio.

Podemos subir los cambios de este repositorio local a un **repositorio remoto en github**, o en otro sitio. Así podemos compartir con todo el mundo escribiendo [código abierto](https://www.redhat.com/es/topics/open-source/what-is-open-source), compartir con nuestro equipo, o compartir con pocas personas de forma privada.

## ¿Qué es Github?

[Github](https://github.com/) es un sitio web y servicio en la nube que facilita a desarrolladores el almacenamiento o _hosting_ de repositorios, así como una forma sencilla de llevar un seguimiento de los cambios hechos en su código.

Aunque Github no solo se emplea en proyectos de código, se ha empleado para llevar todo tipo de proyectos, como [escribir libros](https://braythwayt.com/2015/01/29/how-i-write-books-with-github-and-leanpub.html).

Cualquiera puede registrarse y hostear repositorios públicos o privados de manera gratuita.

De esta forma, podemos resumir que **Github es la plataforma en la nube, donde subimos nuestro código escrito locamente, en nuestras computadoras, mediante Git**.

![Github en la nube, git en la computadora](https://storage.googleapis.com/campus-cvs/guia-code/git-vs-github.png)