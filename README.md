Laravel Schema
===================


This package will help to display database schema information from terminal.

----------


Installation
-------------
Via Composer

``` bash
$ composer require thedevsaddam/laravel-schema 1.0.2
```
Install manually (add the line to composer.json file)
``` bash
"thedevsaddam/laravel-schema": "1.0.*"
```
Open your terminal and hit the command
```bash
composer update
```

Add the following line to config/app.php file

```bash
Thedevsaddam\LaravelSchema\LaravelSchemaServiceProvider::class,
```

### **Usage**
To see the schema information in tabular form
```bash
 php artisan schema:show
```

Schema information in tabular form

![database info commandline](https://raw.githubusercontent.com/thedevsaddam/laravel-schema/master/screenshots/tabular.png)

If you want to see a specific table then pass table  name as first argument
```bash
 php artisan schema:show tableName
```

![database info commandline](https://raw.githubusercontent.com/thedevsaddam/laravel-schema/master/screenshots/tabular-single.png)


Note: Same condition will be applied for tables list view

To see the schema information in list
```bash
 php artisan schema:list
```

Schema information in list

![database info commandline](https://raw.githubusercontent.com/thedevsaddam/laravel-schema/master/screenshots/list.png)

To see the tables name only
```bash
 php artisan schema:simple
```

Tables name with rows count

![database info commandline](https://raw.githubusercontent.com/thedevsaddam/laravel-schema/master/screenshots/simple.png)


To see the table definition
```bash
 php artisan schema:table tableName
```

Table definition with default page and limit

![database info commandline](https://raw.githubusercontent.com/thedevsaddam/laravel-schema/master/screenshots/table-pagination.png)

Note: Provide first argument as **page number** and second argument as **limit** (Both are optional and integer)

To perform raw sql query
```bash
 php artisan schema:query "your sql query"
```

Query result will be dumped in console

![database info commandline](https://raw.githubusercontent.com/thedevsaddam/laravel-schema/master/screenshots/raw-query.png)

Note: Multiple database facility coming soon...

Thank you :)