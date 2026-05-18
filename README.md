# Meeting AI System

Combined Laravel 11 + Vue 3 project.

## Local setup

```bash
composer install
npm install
cp .env.example .env
php artisan key:generate
php artisan migrate --seed
npm run build
php artisan serve
```

For frontend development, run Vite separately:

```bash
npm run dev
```

The Vue app is in `resources/js`, and Laravel serves it through `resources/views/app.blade.php`.

## API

The frontend calls the API at `/api` by default. Set `VITE_API_BASE_URL` only if the API is hosted on a different domain.
