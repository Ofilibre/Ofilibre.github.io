---
title: Publicación de software libre
logo: software-libre/logo.png
date: 2022-04-19
published: true
type: guias
---

[Borrador: documento no definitivo, en proceso de revisión]

Cualquier miembro de la comunidad universitaria puede querer publicar
como software libre un programa que haya realizado. Esta guía explica
cómo hacerlo.

[Aclaración: La palabra "programa" en esta guía se refiere a un programa
de ordenador, o una parte de él. Puede referirse, por lo tanto, tanto
a un programa completo, como una biblioteca o módulo.]

## Cómo publicar software libre

Si decides publicar un programa como software libre, los pasos a seguir
son los siguientes:

* Comprobar que tienes la propiedad intelectual del programa.
* Elegir la licencia de distribución del software.
* Marcar el software como software libre.
* Publicar el software

Vamos a ver estos pasos con más detalle.

## Comprobación de propiedad intelectual

El primer paso es asegurarse de que tienes la propiedad intelectual
del programa. Sólo puedes publicar el programa, y hacerlo con la
licencia de tu elección, si tienes la propiedad intelectual sobre él.

Hay algunos casos en que esto es claro:

* Si eres un alumno y has realizado tu programa con independencia
razonable. En particular, si has hecho por tu cuenta programas para
tu TFG.

Si tienes dudas sobre la propiedad intelectual del programa, consulta
con la OfiLibre.

## Elección de licencia

El siguiente paso para publicar tu programa como software libre
es elegir una licencia de software libre.

Quien tiene la propiedad intelectual de un programa tiene
todos los derechos sobre él. Quien recibe
esa programa sólo puede ejercer los derechos que su propietario
le haya otorgado. Quien recibe el programa
no puede reproducirlo, ni redistribuirlo,
ni realizar una obra derivada
(como corregir un error o añadirle funcionalidad), por ejemplo,
salvo que consiga permiso del autor.

En el caso de la publicación como software libre
la licencia es el texto que indica qué permisos estás
otorgando a quien reciba tu programa, automáticamente
y sin que te tenga que pedir permiso específicamente.
En general, estos permisos incluirán los que detallan
las definiciones más habituales de software libre:
la [Free Software Definition](https://www.gnu.org/philosophy/free-sw.en.html#fs-definition) y la [Open Source Definition](https://opensource.org/osd).

Por ejemplo, la Free Software Definition indica que:

> «Software libre» es el software que respeta la libertad
> de los usuarios y la comunidad. A grandes rasgos, significa
> que los usuarios tienen la libertad de ejecutar, copiar,
> distribuir, estudiar, modificar y mejorar el software.

Hay muchas licencias que cumplen estas definiciones. Entre ellas,
algunas de las más habituales son:

* [GNU General Public License (GPL)](https://opensource.org/licenses/GPL-3.0)
* [GNU Lesser General Public License (LGPL)](https://opensource.org/licenses/LGPL-3.0)
* [Apache License](https://opensource.org/licenses/Apache-2.0)
* [MIT License](https://opensource.org/licenses/MIT)
* [BSD License}(https://opensource.org/licenses/BSD-3-Clause)

Puedes consultar también la [lista de todas las licencias reconocidas por OSI](https://opensource.org/licenses/category).

## Marcado con la licencia elegida

Una vez sabemos qué licencia vamos a usar, tenemos que marcar
el programa con esa licencia. Para ello, normalmente se marca el
código fuente de varias maneras:

* Poniendo en las cabeceras de todos los ficheros fuente un texto que hace referencia a la licencia. Se considera una buena práctica utilizar el [identificador SPDX](https://spdx.dev/ids/) de la licencia, que puede obtenerse, por ejemplo, de la descripción de la licencia en el [listado de licencias de OSI](https://opensource.org/licenses/category). Por ejemplo, en las primeras líneas de un fichero Python:

```
# Copyright 2022 Pepita Menganez
# SPDX-License-Identifier: GPL-3.0
```

* En el directorio principal del código fuente del programa, incluir un fichero `LICENSE` con el texto de la licencia.

* Si el programa tiene una interfaz de usuario, incluir en ella alguna forma en que indique la licencia. Por ejemplo, si tiene una interfaz gráfica de usuario basada en menús, se puede poner una opción de menú "Acerca de" que muestre, entre otra información, la licencia de distribución.


Y con esto estaremos listos para el último paso.

## Publicación

El proceso termina con la publicación del programa. Hoy día
es habitual publicar el proyecto en [GitHub](https://github.com) o
[GitLab](https://gitlab.com), pero cualquier sitio que tenga
vocación de mantenerse en el tiempo, y que esté archivado por
recopiladores como [Software Heritage])(https://www.softwareheritage.org/)
puede servir.

En caso de que el software acompañe a un artículo, una memoria de TFG,
o cualquier otro documento, será conveniente incluir el enlace (URL)
al repositorio donde lo has depositado en ese documento.

## Más información

Esta guía no es más que un resumen brevísimo de algunos pasos imprescindibles para publicar software libre. Puedes profundizar en el tema de la liberación de programas como software libre en los siguientes documentos:

* [Starting an open source project (Open Source Guide)](https://opensource.guide/starting-a-project/)
* [Starting an open source project (Linux Foundation)](https://www.linuxfoundation.org/tools/starting-an-open-source-project/#where)

Hay también muchísimos ejemplos programas publicados como software libre, donde puedes ver cómo lo han hecho. Sólo por mencionar uno:

* [GrimoireLab Perceval](https://github.com/chaoss/grimoirelab-perceval)



