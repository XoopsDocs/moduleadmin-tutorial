# Configuration of xoops\_version.php

In order to use the Framework, you have to add the lines below in your xoops\_version.php :

To list authors:

```php
$modversion['author'] = 'Author1,Author2,Author3';
```

You can set as much authors of the module as you want, but it is necessary to separate them with a comma.

```php
$modversion['nickname'] = 'Pseudo1,Pseudo1,Pseudo3';
```

You must put the same number of usernames used for authors Username1 = Author1, etc. Usernames are separated with a comma.

```php
$modversion['website'] = 'www.website.com'; 
$modversion['name_website'] = 'website';
```

For the variable website, you must put the url of your site and for the variable name\_website, it is necessary to put the title of your website

```php
$modversion['license'] = 'GNU GPL'; 
$modversion['license_url'] = 'www.gnu.org/licenses/gpl-2.0.html/';
```

For the variable license, you must put the type of license and for the variable license\_url, it is necessary to put the url of the license.

```php
$modversion['status_version'] = 'status';
```

You must indicate the status of your module. The standard status options are the following :

* **Alpha**: The Alpha versions are the first versions of the module, lot of bugs exist in such versions and lot of features are still missing. Therefore this version should NOT be used on a production Website. 
* **Beta**: The versions Beta are more advanced than Alpha. Bugs exist again, but almost all the features of the module are present. Also this version should NOT be used on a production Website. 
* **RC**: Which means "Release Candidate", the RC versions they are enough advanced to be distributed to any user. It is not advisable to use them in a productive website. 
* **Final**: This is the final version of the module it can be installed and used in a production website. 

All the version status names, except the Final one, can be followed by a number \(e.g. Beta 1, Beta 2\) to differentiate between versions.

For the overall module versioning, we highly recommend to follow the [**"Semantic Versioning"**](http://semver.org/) schema:

> Given a version number MAJOR.MINOR.PATCH, increment the:
>
> 1. MAJOR version when you make incompatible API changes,
> 2. MINOR version when you add functionality in a backwards-compatible manner, and
> 3. PATCH version when you make backwards-compatible bug fixes.
>
> Additional labels for pre-release and build metadata are available as extensions to the MAJOR.MINOR.PATCH format.

```php
$modversion['release_date'] = 'year/month/day';
```

Date of the publication of the version. This date must have the format: 'year/month/day'

The Framework will handle automatically the translation of the date in the appropriate format according the website language.

```php
$modversion['help'] = 'page=help';
```

Allow you to specify the template of the help page of the module also to create the help menu.

```php
$modversion['min\_php'] = '5.4';
```

Vou have to specify the minimum php version required to a good working of the module. Anyway, you need at least 5.2, because the Framework does not work on an earlier version.

```php
$modversion['min\_xoops'] = '2.5.7';
```

You have to specify the minimum xoops version required to a good working of the module. Anyway, you need at least 2.5, because the Framework does not work on an earlier version.

```php
$modversion['system_menu'] = 1;
```

Since the version 2.5 of XOOPS, the system module generates automatically the administration menu if we add this line.

All these parameters are required to use the Framework.

