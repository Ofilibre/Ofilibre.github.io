---
title: "Convocatoria de asignaturas en abierto: software para docencia"
logo: software-libre/logo.png
date: 2022-09-06
published: true
type: guias
---

[Borrador: documento no definitivo, en proceso de revisión]

La convocatoria de [Reconocimiento de publicación de asignaturas en abierto](/guias/convocatoria-asignaturas-abierto) permite que los docentes aporten, en la categoría "Otros materiales" software (programas de ordenador) utilizado en la docencia: prácticas resueltas, programas de ejemplo, programas realizados para facilitar la comprensión de aspectos de la asignatura, etc. Esta guía proporciona algunas recomendaciones sobre cómo presentar este tipo de software para su consideración en dicha convocatoria.

## Características

Para ser considerado entre los materiales de acceso abierto aportados para la consideración de una asignatura (categoría "Otros materiales"), siguiendo los principios de la convocatoria, deberían cumplirse las siguientes características:

* El software está disponible en un repositorio público, en uno de los formatos aceptados por [Software Heritage](https://softwareheritage.org) (por ejemplo, git, svn o bzr).
* El software se utiliza en la asignatura que se presenta a la convocatoria durante el curso 2022-2023.
* Al menos uno de los docentes que imparte la asignatura es también autor o autora del software presentado.
* El software incluye instrucciones sobre cómo usarse, o estas instrucciones están en algún otro material de acceso abierto utilizado en la asignatura.
* El código fuente de todo el software que se presenta está incluido en el depósito, y está correctamente licenciado con una licencia reconocida por OSI.

## Depósito

Pasos a seguir para depositar software, de forma que pueda considerarse en la categoría "Otros materiales" de la Convocatoria de Reconocimiento de Asignaturas en Acceso Abierto:

* Preparación del repositorio, incluyendo un fichero `README.md`.
* Depósito en [Software Heritage](https://softwareheritage.org).
* Obtención del identificador de Software Heritage para la versión que se presente, y de un fichero comprimido con los contenidos correspondientes.
* Subida a [BURJC Digital](https://burjcdigital.urjc.es) (DSpace) del fichero README.md  en formato PDF, con el fichero comprimido como adjunto, incluyendo el identificador de Software Heritage y la URL del repositorio público en los metadatos.

Al terminar este proceso, se podrá ya incluir en el formulario de solicitud de la convocatoria los datos del software depositado (ver al final de esta guía).

NOTA: tanto el depósito en Software Heritage como la obtención del identificador y el fichero comprimido puede realizarse más cómodamente con la [extensión de Software Heritage para el navegador](https://www.softwareheritage.org/browser-extensions/)

A continuación se detallan estos pasos.

## Preparación del repositorio

Antes de depositar el software, hay que preparar un repositorio público que será el que luego se archive y deposite:

* Si el software ya está en un repositorio público en un servicio de alojamiento de software (como [GitHub](https://github.com) o [GitLab](https://gitlab.com), por ejemplo), puedes preparar ese repositorio, atendiendo a las instrucciones que se detallan a continuación. Si no es así, primero tendrás que subir el software a alguno de estos servicios. Si no sabes cómo hacerlo, puedes seguir el mini-curso de GitHub ["Uploading your project to GitHub"](https://lab.github.com/githubtraining/uploading-your-project-to-github) o la [documentación "Repository" de GitLab](https://docs.gitlab.com/ee/user/project/repository/).

* Prepara un fichero `README.md` en formato Markdown (o simplemente en formato texto plano) describiendo los contenidos del repositorio, de forma que pueda entenderse su función docente, y que puedan ser utilizados por una persona interesada en utilizarlos para aprender.

* Prepara un fichero `LICENSE` o `COPYING`, con la licencia utilizada, que tendrá que ser una de las reconocidas por [OSI (Open Source Initiative)](https://opensource.org/) como licencia "open source" (ver [listado de licencias reconocidas por OSI](https://opensource.org/licenses/category)). En la medida en que sea apropiado para el caso concreto, se recomiendo utilizar una licencia de la categoría "popular and widely-used or with strong communities".

* Recomendación: marcar la cabecera de todos los ficheros fuente con al nota de copyright indicando la fecha y la autoría, y el [identificador SPDX](https://spdx.org/licenses/) de la licencia utilizada. Por ejemplo, para un fichero Python distribuido bajo la licencia GNU GPL 3.0 o posterior: 

```
__copyright__ = "Copyright (C) 2022 Nombre Apellidos"
__license__ = "GPL-3.0-or-later"
```

* Recomendación: Ordenar los contenidos del repositorio en directorios, de forma adecuada para su uso,  e incluir documentación o referencias a la documentación del software.

## Depósito en Software Heritage:

El depósito en Software Heritage comenzará por comprobar si ya está depositado allí (porque es muy posible que ya se haya hecho automáticamente), en la versión concreta que se presenta a la convocatoria. Si no fuera así, se forzará el depósito:

* Si el software está ya en un repositorio de GitHub o GitLab es muy posible que ya esté archivado en Software Heritage, con lo quizás no haga falta realizar este paso. En cualquier caso, para asegurarse de que está archivado de forma adecuada, es mejor actualizar primero el repositorio, y luego realizar el depósito de esa versión en Software Heritage.

* Seguir instrucciones en ["Save code now"](https://archive.softwareheritage.org/save/) para depositar el software.

## Obtención de identificador y fichero comprimido

Para obtener el SWHID de la versión que se presentará a la convocatoria, y de un fichero comprimido con los contenidos depositados:

* Una vez depositado en Software Heritage, busca el repositorio en el [formulario de búsquedas de Software Heritage](https://archive.softwareheritage.org/browse/search). Localiza en él la versión que quieres: Pulsa sobre "History" para ver todas las versiones (commits) archivadas en Software Heritage, y localiza la que quieres presentar a la convocatoria.

* Una vez has localizado la versión concreta, pulsa "Download". En un momento comenzará la descarga de un fichero con extensión `tar.gz`, que contendrá todos los ficheros depositados en esa versión, comprimidos. Este es el fichero comprimido que tendrás que subir a BURJC Digital. El nombre del fichero te dará el SWHID: será el nombre del fichero que ha generado Software Heritage, quitanto `.tar.gz` y sustituyendo "_" por ":". Por ejemplo, este es un SWHID: `swh:1:dir:46dfa1d1d13ae5a725c4ff53f2714f1d237fff7d`.

## Subida a BURJC Digital

Para terminar el proceso, tendrás que subir el fichero comprimido a [BURJC Digital](https://burjcdigital.urjc.es), el Archivo Abierto de la URJC:

* Crea un fichero PDF que tenga los mismos contenidos que el fichero README.md (o README) de la versión del repositorio que vas a subir. Puedes hacerlo de muchas formas:


  * Utilzando un servicio de conversión, como por ejemplo [MARKDOWNtoPDF](https://www.markdowntopdf.com/).

  * Copiando el texto en un editor y guardando en PDF desde él (en este caso, mejor copia respetando el formato la versión HTML que te proporcionan GitLab o GitHub).

  * Desde el IDE, si tienes opción de guardar como PDF un documento Markdown (puede que te haga falta instalar alguna extensíón).

  * Utilizando [pandoc](https://pandoc.org/). Después de instalarlo, ejecuta: 
```
pandoc README.md -s  -f gfm -V colorlinks=true -o README.pdf
```

* Sigue las [instrucciones de BURJC Digital](https://burjcdigital.urjc.es/page/howtopublish) para realizar el archivo:

  * Elige la colección "materiales docentes", y en el campo "Resumen", escribe un resumen sobre el software que estás subiendo, y termina con estas dos líneas (sustituyendo, naturalmente, por el identificador en Software Heritage de tu versión, y la url de tu repositorio público): 

```
> SWHID: {Identificador de Software Heritage}
> Repositorio: {url del repositorio público}
```

  * Sube como documento a depositar el fichero PDF que has generado anteriormente.

  * Incluye como fichero adjunto el fichero comprimido que descargaste de Software Heritage.


## Referencia en el formulario de solicitud:

En el formulario de solicitud de la Convocatoria de Reconocimiento de Asignaturas en Acceso Abierto, en el apartado correspondiente a la categoría "Otros materiales":

* Escribe la url de BURJC Digital.

* Escribe un texto explicando cómo crees que el software cumple los criterios de evaluación, como harías con, por ejemplo, los apuntes de la aisgnatura.

## Extensión de Software Heritage para el navegador.

Puede instalarse tanto en Firefox como en Chrome la [extensión de Software Hertiage](https://www.softwareheritage.org/browser-extensions/), que permite comprobar cómodamente el estado de archivo de un repositorio alojado en GitHub o GitLab, pedir la actualización del archivo, conseguir su SWHID, o incluso el fichero comprimido con sus contenidos.

## Referencias

Puede ser útil, antes de componer el repositiro, consultar la guía [Publicación de software libre](/guias/publicar-software-libre).