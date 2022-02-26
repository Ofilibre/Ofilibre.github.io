---
title: "Autenticación de dos factores con FreeOTP"
date: 2022-02-26
slug: freeotp-2factores
draft: false
author: "OfiLibre"
type: "post"
tags: ["software libre", "autenticación", "URJC"]
categories: ["software libre"]
description: "FreeOTP es un programa libre que puede funcionar como segundo factor de autenticación"

# post images 
bg_image: "images/blog/freeotp-2factores/square.png"
thumb: "images/blog/freeotp-2factores/square.png"
---

En la URJC estamos de transición al [uso de varios factores de autenticación](https://infotic.urjc.es/pages/viewpage.action?pageId=135299113) (la contraseña y otro) para poder utilizar muchos servicios. El segundo factor puede por ejemplo un móvil, donde recibiremos un código que tendremos que introducir para autenticarnos. Pero puede ser también una aplicación, normalmente para el móvil, que nos dará el código para autenticarnos. 

Hay varias aplicaciones libres que proporcionan esta funcionalidad. Entre ellas destaca [FreeOTP](https://freeotp.github.io/), que puedes descargar para Android o iOS. Esta aplicación, además de para autenticarnos en los servicios Office365 contratados por la Universidad (correo electrónico, Teams, OneDrive, etc.) sirve también para otros muchos servicios que utilizan el estándar [TOTP](http://www.ietf.org/rfc/rfc6238.txt) para atender a un segundo factor de autenticación, como GitHub, GitLab, Google, Amazon o Facebook.

La configuración de FreeOTP para Office365 es muy sencilla. Sigue las recomendaciones de la [infografía proporcionada por CIED](https://online.urjc.es/contenidos/urjconline/mailing/doble-factor-de-autenticacion-en-office365.pdf), en la parte que explica cómo configurar Microsoft Authenticator, pero usando FreeOTP como aplicación. En resumen:

* Descarga FreeOTP en tu móvil ([versión Android en F-Droid](https://f-droid.org/packages/org.fedorahosted.freeotp/), [versión Android en Google Play](https://play.google.com/store/apps/details?id=org.fedorahosted.freeotp), [versión iOS](https://apps.apple.com/us/app/freeotp-authenticator/id872559395)).

* En tu ordenador, accede a las [opciones de seguridad de tu cuenta en Office365](https://mysignins.microsoft.com/security-info). En el panel "Información de seguridad", pulsa en la opción "Añadir un método". Cuando te indica que obtengas "Microsoft Authenticator", elige "Quiero usar una aplicación de autenticación diferente". Cuando sale el panel indicando "Configura tu aplicación", pulsa en "Siguiente" para ver un código QR.

* En el móvil, lanza FreeOTP y pula en el icono de la cámara (esquina inferior derecha). Podrás ahora escanear el código QR de la pantalla de tu ordenador, con la cámara del móvil. Eso te configurará FreeOTP para poder autenticarte, en cuanto aceptes en el móvil el mensaje que te indica que estás añadiendo un nuevo servicio. En la pantalla principal de FreeOTP te aparecerá a partir de ahora un icono con el logo de Microsoft.

Ahora, cuando te autentiques en los servicios de Office365 de la Universidad, cuando además de tu contraseña te pidan un código, lanza FreeOTP en tu móvil, pulsa sobre el logo de Microsoft, e introduce el código que te da la aplicación.

Puedes aprovechar para configurar un segundo factor de autenticación usando FreeOTP con otros servicios, ya que estamos...

FreeOTP es software libre, así que si quieres, puedes ver su [código fuente](https://github.com/freeotp), y adaptarlo a tus necesidades si sabes programar.