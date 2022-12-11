# Laravel Quick Guide - For Rapid Project Development. 

## Purpose 
Step by Step Process - Skipping Explaination. 

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
npm run dev
```

### Changing Logo (Inertia)
Change the content of the following Path. 

Expect a SVG.

```
/resources/applicationMark.vue 
```

