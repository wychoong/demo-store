<p align="center"><a href="https://getcandy.io/" target="_blank"><img src="https://getcandy.io/getcandy_logo.svg" width="400" alt="GetCandy"></a></p>

# Demo Store

This repository is provided as a reference to learn how to use GetCandy Laravel E-Commerce package. It is a classic e-commerce store and we have a [screencast series in the docs](https://docs.getcandy.io/screencasts) which show you how we created each section of the store.

# Requirements

This demo store uses Meilisearch, for the best experience it is recommended you use this as well.

# Installation

## Clone the repo

```bash
git clone --depth=1 https://github.com/getcandy/demo-store.git
```

This will create a shallow clone of the repo, from there you would just need to remove the `.git` folder and reinitialise it to make it your own.

Then install composer dependencies

```bash
composer install
```

## Configure the Laravel app

Copy the `.env.example` file to `.env` and make sure the details match to your install.

All the relevant configuration files should be present in the repo.

## Migrate and seed.

Run the migrations

```
php artisan migrate
```

Install GetCandy

```
php artisan getcandy:install
```

Seed the demo data.

```
php artisan db:seed
```

---

This demo store uses Livewire to handle all routing and Laravel components where they make sense.
