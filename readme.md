# Laravel Quick Guide - For Rapid Project Development. 

## Purpose 
Step by Step Process - Skipping Explaination. 

# Setup

## Installing Laravel Dependencies. 

### Composer

[Download Composer Installer](https://getcomposer.org/Composer-Setup.exe)


## Installation Laravel

``` composer create-project laravel/laravel example-app ```

## Running Project. 

``` 
php artisan serve
```

## Installing Jet Stream. 

``` 
composer require laravel/jetstream 
```

## Installing inertia

``` 
php artisan jetstream:install inertia --teams 
```

### Finalizing Installation. 

``` 
npm install
npm run build
php artisan migrate
```

## Running Development for Hot Reload (VueJs/Inertia) 

Quick Tip - Run it on a different cmd prompt with ``` php artisan serve ```

```
> npm run dev
```

# Tasks Post Setup

## 1.  Changing Logo (Inertia)
Change the content of the following Path. 
```
/resources/applicationMark.vue 
```

> Get Quick SVG (emojis)  
> https://www.kirupa.com/tools/twemoji_browser.htm

--- 

## 2. Building Content Type (Example Sites)

### Creating a Model

``` 
php artisan make:model -mrc {{ItemName}}
``` 

Understanding Notes. 

> You can see all the available options by running the ``` php artisan make:model --help ``` command.

>[ Model from Laravel Bootcamp  ](https://bootcamp.laravel.com/inertia/creating-chirps )


### Creating Routes

Open ```(Ctl + P)```

```
web/routes.php
```

Add at top to routes.php

```
use App\Http\Controllers\{{ItemName}}Controller;
```

Add Route to routes.php

```
Route::resource('chirps', {{ItemName}}Controller::class)
    ->only(['index', 'store'])
    ->middleware(['auth', 'verified']);
```

Check with ``` php artisan route:list ```







## References & Resources. 

[Laravel Bootcamp](https://bootcamp.laravel.com/inertia/installation)
[Laravel CRUD](https://larainfo.com/blogs/laravel-9-inertia-vue-3-crud-tutorial-example)










