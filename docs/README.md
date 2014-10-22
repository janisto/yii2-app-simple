Yii 2 Simple Application Template
================================

Yii 2 Simple Application Template is a skeleton Yii 2 application best for
rapidly creating multiple simple projects in subfolders using LAMP stack.

The template contains the basic features including user login/logout and a contact page.
It includes all commonly used configurations that would allow you to focus on adding new
features to your application.


DIRECTORY STRUCTURE
-------------------

      protected/assets/             contains assets definition
      protected/commands/           contains console commands (controllers)
      protected/config/             contains application configurations
      protected/controllers/        contains Web controller classes
      protected/mail/               contains view files for e-mails
      protected/models/             contains model classes
      protected/runtime/            contains files generated during runtime
      protected/tests/              contains various tests for the basic application
      protected/views/              contains view files for the Web application
      vendor/                       contains dependent 3rd-party packages
      /                             contains the entry script and Web resources



REQUIREMENTS
------------

The minimum requirement by this application template that your Web server supports PHP 5.4.0.

You can also check if your server configuration meets the requirements for
running Yii application by executing the following command after installation:

~~~
php protected/requirements.php
~~~

INSTALLATION
------------

### Install from an Archive File

Extract the archive file downloaded from [github.com](https://github.com/janisto/yii2-app-simple/releases) to
a directory named `simple` that is directly under the Web root.

You can then access the application through the following URL:

~~~
http://localhost/simple/
~~~


### Install via Composer

If you do not have [Composer](http://getcomposer.org/), you may install it by following the instructions
at [getcomposer.org](http://getcomposer.org/doc/00-intro.md#installation-nix).

You can then install this application template using the following command:

~~~
php composer.phar global require "fxp/composer-asset-plugin:1.0.0-beta3"
php composer.phar create-project --prefer-dist janisto/yii2-app-simple simple
~~~

Now you should be able to access the application through the following URL, assuming `simple` is the directory
directly under the Web root.

~~~
http://localhost/simple/
~~~


CONFIGURATION
-------------

### Database

Edit the file `protected/config/db.php` with real data, for example:

```php
return [
    'class' => 'yii\db\Connection',
    'dsn' => 'mysql:host=localhost;dbname=yii2_simple',
    'username' => 'root',
    'password' => '1234',
    'charset' => 'utf8',
];
```

**NOTE:** Yii won't create the database for you, this has to be done manually before you can access it.

Also check and edit the other files in the `protected/config/` directory to customize your application.
