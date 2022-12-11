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

