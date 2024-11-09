# Lite SSR

This repo is a report for SSR issue on Inertia + Svelte 5. The problem happens after user logged in.

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

## Summary

I toggle on/off for Enabled JavaScript in my browser (I use Safari) to test SSR. It works on landing page, login page, and register page. But, it doesn't work after user logged in (Dashboard page). I get an error message.

```sh
Unhandled Promise Rejection: HierarchyRequestError: The operation would yield an incorrect node tree.
```
