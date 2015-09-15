---
language: Español
currentMenu: guarda_articulo
subTitle: Guarda tu primer artículo
---

# Guarda tu primer artículo

Una vez conectado a wallabag, puedes guardar artículos de diversas maneras.

## En la web de wualla

En el menú tienes un enlace **guardar un enlace**. Pulsando en él, aparece un formulario: sólo tienes que escribir la dirección del artículo que quieres guardar.

Confirma para guardar el contenido del artículo.

Por defecto, sólo el texto se guarda. Sí quieres guardar una copia de las imágenes en tu servidor, tienes que activar la opción *DESCARGAR IMÁGENES*. Lee el capitulo sobre opciones ocultas para más información

## Desde el marcador

De la [Wikipedia](http://es.wikipedia.org/wiki/Bookmarklet):

“Un bookmarklet es un marcador que, en lugar de apuntar a una dirección URL, hace referencia a una pequeña porción de código JavaScript para ejecutar ciertas tareas automáticamente, como por ejemplo:

* Cambiar el diseño de la página (el tamaño de letra o los colores, quitar el fondo, etc.).
* Mostrar información de enlaces, imágenes, formularios, etc.).
* Abrir una consulta directamente en un motor de búsqueda o acerca del texto que hayamos seleccionado.”

En el menú de wallabag, pulsa en **configuración**. Al inicio de la página hemos listado todas las formas para guardar un artículo. Encontrarás el marcador  (es el enlace `¡embólselo!`) para arrastrar y soltar el la barra de marcadores de tu navegador.

De ahora en adelante, cuando quieras guardar la página que estas leyendo, sólo tienes que pulsar en este marcador y el artículo será automáticamente guardado.

## Desde tu smartphone

### Primero de todo

Para usar la aplicación pará móvil, tienes primero que activar los feeds RSS desde la configuración de wallabag. Entonces cierta información será mostrada, cómo nuestro token de seguridad. Lee el capitulo sobre feeds RSS para más información.

### Android

#### Instalación y configuración

Puedes descargar la aplicación desde la [Google Play Store](https://play.google.com/store/apps/details?id=fr.gaulupeau.apps.InThePoche) y desde [F-droid](https://f-droid.org/app/fr.gaulupeau.apps.InThePoche). Es exactamente la misma aplicación en ambas tiendas.

Una vez instalada, arranca la aplicación, ve a la **configuración** y introduce la  **URL (dirección completa de tu instalación de wallabag o tu cuenta en Framabag)** y **User ID (normalmetne, tendrás que poner 1)**. Sí has creado múltiples cuentas desde wallabag, tendrás que introducir el usuario que quieres conectar a la aplicación y tu **Token** de seguridad (introduce correctamente el token cómo se ve en la página de configuración de wallabag).

#### Guardar un artículo

Ahora que esta todo configurado, puedes compartir un artículo desde el menú de  **Compartir**: encontrarás un **¡embólselo!** que añadirá tu artículo a wallabag.

#### Leer

Cuando abres la aplicación, pulsa en sincronizar: tus artículos recientemente guardados serán añadidos a tu smartphone.

A partir de aquí ya no necesitas una conexión a internet: pulsa en **Mostrar artículos** para empezar a leer.

Al final de cada artículo, hay un botón **Marcar cómo leído** que te permite archivarlo.

Hasta ahora, la sincronización ocurre en una dirección (desde wallabag hacia la app), previniendo marcar un artículo cómo leído desde tu smartphone.

### iOS

#### Installation and configuration

You can download the iOS application from the [AppStore](https://itunes.apple.com/app/id828331015).

Once installed, configure the app by filling following fields inside the settings: the **URL (complete address of your wallabag installation or your Framabag account)** and **User ID (in most cases, you'll have to put 1)** field. If you have created multiple accounts from wallabag, you will have to to fill the user account you want to connect to your application and your security **Token** (enter properly all the token's letters as seen in the settings part of wallabag).

#### Usage

If the app is configured correctly, the app will automatically download the articles from your wallabag (use **pull-to-refresh** to trigger this update manually). Once an article is downloaded, it'll be available offline from your app.

Unfortunately you can only locally mark an article as read (it will not synchronise to your online wallabag).

### Saving articles

If you're browsing a website and want to add the current article to your wallabag, simply tap the **Share**-button and select **Bag it!** (if you don't find the wallabag icon, have a look in the **more**-menu). If everything is set up correctly, your article will be saved (you may have to login from time to time).

###Windows Phone
####Installation and configuration

You can download the Windows Phone application from the [Windows Store](https://www.microsoft.com/en-us/store/apps/wallabag/9nblggh11646) or directly from your smartphone's Store.

Once installed, the application will show you a notification on the first launch, asking the configuration of your wallabag server. Go to the **Settings** part of the application by pressing the three dots menu at the bottom of the screen, then fill in the **URL (complete address of your wallabag installation or your Framabag account)** and **User ID (in most cases, you'll have to put 1)** fields.

If you have created multiple accounts from wallabag, you will have to to fill the user account you want to connect to your application and your security **Token** (enter properly all the token's letters as seen in the setting part of wallabag).

## From your web browser

### Firefox Classic Add-on

Download the Firefox add-on at [addons.mozilla.org](https://addons.mozilla.org/firefox/addon/wallabag/) and install it like any other Firefox add-on.

In the add-on's settings, fill the complete URL of your installation of wallabag or your Framabag account.

Personalize the Firefox toolbar to add wallabag (**W** icon). When you find an article you want to save, click on this icon: a new window will open to add the article and will close itself automatically.

### Firefox Social API Service

*Available from wallabag v1.9.1 only*

*You will need an https connection to use this. It's a Firefox [requirement](https://developer.mozilla.org/en-US/docs/Mozilla/Projects/Social_API/Manifest#Manifest_Contents), sorry*

With Firefox 29+ versions, your browser comes with an integrated interface to share things to multiple social services directly from your browser. In the Firefox interface, it is shown a paper plane-like icon that you will use to share a page, which means here, save an article.
You can add the service by going into the Config page of wallabag, then click on Mozilla Services Social API Extension. You must also accept to use Firefox Services.

### Chrome

Download the Chrome add-on [on the dedicated website](https://chrome.google.com/webstore/detail/wallabag/bepdcjnnkglfjehplaogpoonpffbdcdj) and install it like any other Chrome add-on.

In the add-on's settings, fill the complete URL of your installation of wallabag or your Framabag account.

During the addon's installation, a new icon appear in Chrome toolbar (a **W** icon). When you find an article you want to save, click on this icon: a popup will appear to confirm that your article has been saved.

### Opera

The recent versions of Opera (15+) allow to install add-ons compatible with Chrome.

First, install the add-on named [Download Chrome Extensions](https://addons.opera.com/en/extensions/details/download-chrome-extension-9/) which will allow you to install add-ons from the Chrome Web Store. Then, go [to to Google site](https://chrome.google.com/webstore/detail/wallabag/bepdcjnnkglfjehplaogpoonpffbdcdj) and get the Chrome add-on by clicking on *Add to Opera*. A message will invite you to confirm this action because this add-on is not coming from a certified source. The behavior will be the same as for Chrome (see above).
