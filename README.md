Yii 2 Basic Practical Application Template
================================

Yii 2 Basic Practical Application Template is a skeleton Yii 2 application best for
rapidly creating small projects.

The template contains the basic features including user login/logout and a contact page.
It includes all commonly used configurations that would allow you to focus on adding new
features to your application.

Also, the Yii 2 Basic Practical Application Template has a structure that is compatible with
almost all hosting provider, so that you won't have to worry when pushing your Yii 2 web application
to the Internet.


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
      protected/vendor/             contains dependent 3rd-party packages
      protected/views/              contains view files for the Web application
      /                             contains the entry script and Web resources



REQUIREMENTS
------------

The minimum requirement by this application template that your Web server supports PHP 5.4.0.


INSTALLATION
------------

### Install from an Archive File

Extract the archive file downloaded from [github.com/ducntq/yii2-app-basic-practical/releases](https://github.com/ducntq/yii2-app-basic-practical/releases)
to a directory named `basic` that is directly under the Web root.

You can then access the application through the following URL:

~~~
http://localhost/basic/
~~~


### Install via Composer

If you do not have [Composer](http://getcomposer.org/), you may install it by following the instructions
at [getcomposer.org](http://getcomposer.org/doc/00-intro.md#installation-nix).

You can then install this application template using the following command:

~~~
php composer.phar global require "fxp/composer-asset-plugin:1.0.0-beta4"
php composer.phar create-project --prefer-dist --stability=dev ducntq/yii2-app-basic-practical basic
~~~

Now you should be able to access the application through the following URL, assuming `basic` is the directory
directly under the Web root.

~~~
http://localhost/basic/
~~~


CONFIGURATION
-------------

### Database

Edit the file `protected/config/db.php` with real data, for example:

```php
return [
    'class' => 'yii\db\Connection',
    'dsn' => 'mysql:host=localhost;dbname=yii2basic',
    'username' => 'root',
    'password' => '1234',
    'charset' => 'utf8',
];
```

**NOTE:** Yii won't create the database for you, this has to be done manually before you can access it.

Also check and edit the other files in the `config/` directory to customize your application.
