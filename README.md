Easy Install (module for Omeka S)
=================================

> ***IMPORTANT***: This module is deprecated and has been replaced by the module
> [Easy Admin] and won’t be updated any more. The upgrade from it is automatic.

> __New versions of this module and support for Omeka S version 3.0 and above
> are available on [GitLab], which seems to respect users and privacy better
> than the previous repository.__

[![Build Status](https://travis-ci.org/Daniel-KM/Omeka-S-module-EasyInstall.svg?branch=master)](https://travis-ci.org/Daniel-KM/Omeka-S-module-EasyInstall)

[Easy Install] is a module for [Omeka Semantic] that allows to install Omeka S
modules and themes from https://omeka.org and from the web (https://github.com
and https://gitlab.com).

The idea comes from the plugin [Escher] for [Omeka Classic].

See more details on [modules] and [themes].


Installation
------------

Uncompress files in the directory `modules` and rename folder `EasyInstall`.

See general end user documentation for [Installing a module](http://dev.omeka.org/docs/s/user-manual/modules/#installing-modules).

In some cases, your may need to add credentials in your config (omeka file "config/local.config.php"),
depending on your linux distribution:
```php
    'http_client' => [
        // 'adapter' => \Laminas\Http\Client\Adapter\Curl::class,
        'sslcapath' => '/usr/local/etc/ssl/certs',
        'sslcafile' => '/usr/local/etc/ssl/certs/ca.crt',
        // 'sslcapath' => '/etc/pki/tls/certs',
        // 'sslcafile' => '/etc/pki/tls/certs/ca-bundle.crt',
    ],
```

You can find more information on the params in [Laminas help].


Usage
-----

Simply select either the desired module or the desired theme and click "upload".


Warning
-------

Use it at your own risk.

It’s always recommended to backup and to check your files and database regularly
so you can roll back if needed.


Troubleshooting
---------------

See online issues on the [module issues] page.


License
-------

This plugin is published under the [CeCILL v2.1] license, compatible with
[GNU/GPL] and approved by [FSF] and [OSI].

In consideration of access to the source code and the rights to copy, modify and
redistribute granted by the license, users are provided only with a limited
warranty and the software’s author, the holder of the economic rights, and the
successive licensors only have limited liability.

In this respect, the risks associated with loading, using, modifying and/or
developing or reproducing the software by the user are brought to the user’s
attention, given its Free Software status, which may make it complicated to use,
with the result that its use is reserved for developers and experienced
professionals having in-depth computer knowledge. Users are therefore encouraged
to load and test the suitability of the software as regards their requirements
in conditions enabling the security of their systems and/or data to be ensured
and, more generally, to use and operate it in the same conditions of security.
This Agreement may be freely reproduced and published, provided it is not
altered, and that no provisions are either added or removed herefrom.


Contact
-------

Current maintainers:

* Daniel Berthereau (see [Daniel-KM] on GitLab)


Copyright
---------

* Copyright Daniel Berthereau, 2017-2022


[Easy Admin]: https://gitlab.com/Daniel-KM/Omeka-S-module-EasyAdmin
[Easy Install]: https://gitlab.com/Daniel-KM/Omeka-S-module-EasyInstall
[Escher]: https://github.com/AcuGIS/Escher
[Omeka Semantic]: https://www.omeka.org/s
[Omeka Classic]: https://omeka.org/classic
[Laminas help]: https://docs.laminas.dev/laminas-http/client/adapters
[modules]: https://daniel-km.github.io/UpgradeToOmekaS/omeka_s_modules.html
[themes]: https://daniel-km.github.io/UpgradeToOmekaS/omeka_s_themes.html
[module issues]: https://gitlab.com/Daniel-KM/Omeka-S-module-EasyInstall/-/issues
[CeCILL v2.1]: https://www.cecill.info/licences/Licence_CeCILL_V2.1-en.html
[GNU/GPL]: https://www.gnu.org/licenses/gpl-3.0.html
[FSF]: https://www.fsf.org
[OSI]: http://opensource.org
[GitLab]: https://gitlab.com/Daniel-KM
[Daniel-KM]: https://gitlab.com/Daniel-KM "Daniel Berthereau"
