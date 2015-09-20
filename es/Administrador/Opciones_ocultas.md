---
language: Español
currentMenu: hidden
subTitle: Opciones ocultas
---

# Opciones ocultas

## Peligro

**Ten cuidado**, esta sección esta destinada a usuarios avanzados. El archivo de configuración a modificar, `inc/poche/config.inc.php`, es muy importante. Es recomendable hacer una copia de seguridad del archivo antes de modificarlo.
**Cualquier error en la modificación de este archivo puede dar lugar a fallos de funcionamiento**.

Este archivo es creado durante la instalación de wallabag.
Instala wallabag, haz una copia de seguridad del archivo y luego ya puedes modificarlo con tu editor de texto favorito.

En este archivo hay algunas opciones que por ahora no están disponibles en la página **configuración** de wallabag.

## Modificación de opciones avanzadas

Cada opción esta definida de este modo:

	@define ('OPTION_NAME', 'Valor');

Para cada linea, puedes modificar el campo `Valor`.

Aquí esta la lista de cada opción que puedes cambiar:

* `HTTP_PORT` (por defecto: `80`) : El puerto HTTP de tu servidor web. Puedes ser que lo tengas que cambiar si tu servidor esta tras un proxy. Valores posibles: Número del puerto.
* `SSL_PORT` (por defecto: `443`) : El puerto HTTPS de tu servidor web.  Puedes ser que lo tengas que cambiar si tu servidor esta tras un proxy. Valores posibles: Número del puerto.
* `MODE_DEMO` (por defecto : `FALSE)`: Si quieres montar un servidor de demostración... Valores posibles: `TRUE` o `FALSE`.
* `DEBUG_POCHE` (por defecto: `FALSE`) : Si encuentras algún problema con wallabag, puede ser que te pidamos que actives el modo de debug. Valores posibles: `TRUE` o `FALSE`. Checa los logs en cache/log.txt después de activarlo.
* `ERROR_REPORTING` (por defecto : `E_ALL & ~E_NOTICE`) : Ponlo como `E_ALL` para buscar errores de PHP.
* `DOWNLOAD_PICTURES` (por defecto: `FALSE`) : Permitir a wallabag descargar las imágenes de los artículos que guardas en tu servidor, en lugar de descargar sólo el texto. Preferimos que decidas tú si quieres activar esta característica. Valores posibles: `TRUE` o `FALSE`.
* `REGENERATE_PICTURES_QUALITY` (por defecto : `75`) : Para evitar fallos de seguridad, las imágenes son regeneradas si activas su descarga. Esta opción controla el porcentaje de calidad con el que son guardadas. Aumenta  el número si quieres más calidad y disminúyelo si quieres mayor velocidad de regeneración.
* `SHARE_TWITTER` (por defecto: `TRUE`) : Permitir compartir por Twitter. Valores posibles: `TRUE` o `FALSE`.
* `SHARE_MAIL` (por defecto: `TRUE`) : Permitir compartir por email. Valores posibles: `TRUE` o `FALSE`.
* `SHARE_EVERNOTE`(por defecto : `FALSE`) : Permitir compartir con tu cuenta de Evernote. Valores posibles: `TRUE` o `FALSE`.
* `SHARE_DIASPORA` (por defecto : `FALSE`) : Permitir compartir por Diaspora.
* `DIASPORA_URL` (por defecto : `http://diasporapod.com`) : La URL de tu Diaspora* pod
* `CARROT` (por defecto : `FALSE`) : Como Flattr, es un servicio para dar pequeñas cantidades de dinero a una página web. Aprende más en http://carrot.org/
* `SHARE_SHAARLI` (por defecto: `FALSE`) : Permitir compartir mediante tu instalación de Shaarli (Shaarli es administrador de marcadores que es software libre). Valores posibles: `TRUE` o `FALSE`.
* `SHAARLI_URL` (por defecto: `'http://myshaarliurl.com'`) : Define la URL de tu instalación de Shaarli. Valores posibles: una URL.
* `FLATTR` (por defecto: `TRUE`) : Permitir Flatear un articulo ([Flattr es una plataforma de microdonaciones](http://en.wikipedia.org/wiki/Flattr)). Si un articulo se puede Flattear, un icono se mostrará, permitiéndote hacer una microdonación al autor. Valores posibles: `TRUE` o `FALSE`.
* `SHOW_PRINTLINK` (por defecto: `'1'`) : Permitir imprimir los artículos. Valores posibles: `'1'` para activar o `'0'` para desactivar.
* `SHOW_READPERCENT` (por defecto: `'1'`) : Muestra el porcentaje de progreso del articulo que estas leyendo (funcionando en los temas `default`, `dark`, `dmagenta`, `solarized`, `solarized-dark`). Valores posibles: `'1'` para activar o `'0'` para desactivar.
* `PAGINATION` (por defecto: `'12'`) : Define el número de articulos que se muestran en una lista. Valores posibles: número.
