---
title: Angular + TypeScript + Caddy
description: The default Angular TS starter, utilizing `Caddy` to serve the built single page app
tags:
  - Node
  - Angular 16
  - TypeScript
  - Caddy
---

# Angular + TypeScript + Caddy

This project was originally generated with [`npm init @angular myApp`](https://angular.io/quick-start#create-a-new-angular-app-from-the-command-line)

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/13NBfA?referralCode=ySCnWl)

## ✨ Features

- Angular 16 + TypeScript + Caddy
- Caddy v2

## 💁‍♀️ Local Development

- Install required dependencies with `npm install`
- Run `npm run dev` for a dev server
- Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.

## ❓ Why use `Caddy` when deploying to Railway?

Caddy is a powerful, enterprise-ready, open source web server, and therefore Caddy is far better suited to serve websites than `ng serve` is, using Caddy will result in much less memory and cpu usage compared to serving with `ng serve` (much lower running costs too)

To see how this is achieved with nixpacks, check out the fully documented nixpacks.toml file in this repository

The configuration for Caddy is called a Caddyfile, and you can edit that file to further suite your needs, by default it comes configured to serve a single page app for Angular, and to also gzip the responses

**Relevant Caddy documentation:**

- [The Caddyfile](https://caddyserver.com/docs/caddyfile)
- [Caddyfile Directives](https://caddyserver.com/docs/caddyfile/directives)
- [root](https://caddyserver.com/docs/caddyfile/directives/root)
- [encode](https://caddyserver.com/docs/caddyfile/directives/encode)
- [file_server](https://caddyserver.com/docs/caddyfile/directives/file_server)
- [try_files](https://caddyserver.com/docs/caddyfile/directives/try_files)