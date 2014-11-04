## Be careful
**Attention**, this part is for advanced users only. We'll edit an important file of wallabag, `inc/poche/config.inc.php`, please make a backup of this file before changes.  
**If you make a mistake while editing a wallabag file, your application may be broken.**

This file is created when wallabag is installed.  
Please first install wallabag, make a backup of this file and open it with ~~Sublime Text~~ your favorite editor.

In this file are defined some parameters that you can't change on the wallabag **configuration** page. 

## Advanced options

Each parameter is defined like this:

    @define ('PARAMETER_NAME', 'Parameter value');
    
For each line, you can only change `Parameter value` part. 

TODO explain all the following parameters

Here are all the parameters you can change: 
* `HTTP_PORT` (default value is `80`): Expected value: a digit.
* `SSL_PORT` (default value is `443`): Expected value: a digit. 
* `DEBUG_POCHE` (default value is `FALSE`): Expected values: `TRUE` or `FALSE`.
* `DOWNLOAD_PICTURES` (default value is `FALSE`): Expected values: `TRUE` or `FALSE`.
* `SHARE_TWITTER` (default value is `TRUE`): Expected values: `TRUE` or `FALSE`.
* `SHARE_MAIL` (par défaut, `TRUE`): Expected values: `TRUE` or `FALSE`.
* `SHARE_SHAARLI` (default value is `FALSE`): Expected values: `TRUE` or `FALSE`.
* `SHAARLI_URL` (default value is `'http://myshaarliurl.com'`): Expected value: your Shaarli URL. 
* `FLATTR` (default value is `TRUE`): Expected values: `TRUE` or `FALSE`.
* `SHOW_PRINTLINK` (default value is `'1'`): Expected values: `'0'` to disable, `'1'` to enable.
* `SHOW_READPERCENT` (default value is `'1'`): `'0'` to disable, `'1'` to enable.
* `PAGINATION` (default value is `'12'`): Expected value: a digit. 