# laravel-7-adminlte-3
how to install adminlte 3.4 on laravel 7

## install laravel 7
```
composer create-project -–prefer-dist laravel/laravel=7 laravel-adminlte
```

## install authentication
```
composer require laravel/ui:^2.4
php artisan ui bootstrap --auth
npm i && npm run dev
```

## install adminlte
```
composer require jeroennoten/laravel-adminlte:^3.4
php artisan adminlte:install
npm i && npm run dev

php artisan adminlte:status

php artisan adminlte:install --only=auth_views
```


## change template welcome.blade.php
```
@extends('adminlte::page')

@section('title', 'Dashboard')

@section('content_header')
    <h1>Dashboard</h1>
@stop

@section('content')
    <p>Welcome to this beautiful admin panel.</p>
@stop

@section('css')
    <link rel="stylesheet" href="/css/admin_custom.css">
@stop

@section('js')
    <script> console.log('Hi!'); </script>
@stop
```
