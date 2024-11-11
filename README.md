# Lite SSR

> This repo has been fullfil it's task. The issue has been solved: https://github.com/inertiajs/inertia/issues/2083.

## How to run?

- Git clone

- Copy environment

```sh
cp .env.example .env
```

- Install deps

```sh
composer install
```

- Run artisan

```sh
php artisan key:generate
php artisan migrate
php artisan db:seed
```

- Install NPM deps

```sh
npm install
npm run build
```

- Run `php artisan serve` and `php artisan inertia:start-ssr` in separate tab terminal.
