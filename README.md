# Frappe Vue UI Starter

A simple starter setup for using **Vue 3 + Frappe UI + Tailwind CSS + Vite** inside a Frappe application.

## Included

* Vue 3
* Frappe UI
* Tailwind CSS
* Vite
* Vue Router
* Frappe Proxy
* Lucide Icons
* Hot Reload during development
* Frappe production build configuration

## Setup

Go to your Frappe app:

```bash
cd ~/frappe-bench/apps/<app-name>
```

Clone the starter into the `frontend` folder:

```bash
npx degit SelvanivasK/frappe-vue-ui-starter frontend
```

Move into the frontend:

```bash
cd frontend
```

Install dependencies:

```bash
yarn
```

## Change App Name

Open:

```text
vite.config.js
```

Replace all occurrences of:

```text
<app-name>
```

with your actual Frappe app name.

Example:

```text
<app-name> → frappewithvue
```

## Frappe Development Configuration

For local development, add the following to:

```text
sites/common_site_config.json
```

```json
"ignore_csrf": 1
```

> Use `ignore_csrf` only for local development.

## Run Frappe

From your bench directory:

```bash
cd ~/frappe-bench
bench start
```

## Run Vue

Open another terminal:

```bash
cd ~/frappe-bench/apps/<app-name>/frontend
yarn dev
```

## Build

To build the Vue frontend for Frappe:

```bash
yarn build
```

The build generates the frontend files inside your Frappe app.

You can access the built page through:

```text
/frontend
```


## Credits

Based on the original doppio_frappeui_starter by Gowtham-L.

Modified with updated configuration for Frappe UI, Tailwind CSS, and Vite compatibility.