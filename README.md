<<<<<<< HEAD
# Frontend - Mallqui Gym

Frontend desarrollado con Angular.
=======
# Backend - Mallqui Gym

Backend REST desarrollado con **Laravel 12**.

## Requisitos

- PHP 8.2 o superior.
- Composer.
- MySQL o MariaDB.
>>>>>>> 67c212c22a11ba7ceb65b36bf231372ef27404ca

## Instalación

```bash
<<<<<<< HEAD
npm install
```

## Ejecutar

```bash
ng serve
```

Abrir:

```text
http://localhost:4200
```

## Estructura principal

```text
src/app/
├── component/
│   └── pages/
├── core/
│   ├── guards/
│   ├── interceptors/
│   ├── services/
│   └── ui/
├── models/
├── app.component.ts
├── app.routes.ts
└── auth.service.ts
```

Los componentes de páginas están organizados dentro de `component/pages`, siguiendo la estructura usada en clase.

## Módulos visibles

Dashboard, clientes, membresías, pagos, entrenadores, clases, rutinas, reservas, asistencias, categorías, productos, proveedores, compras, ventas, Kardex, caja, usuarios, auditoría y reportes.

## Conexión con Laravel

El proyecto usa `proxy.conf.json` para enviar las peticiones `/api` al backend Laravel durante el desarrollo.
=======
composer install
copy .env.example .env
php artisan key:generate
```

Configura en `.env`:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=mallqui_gym
DB_USERNAME=root
DB_PASSWORD=
```

## Crear la base de datos del proyecto

El repositorio incluye comandos Artisan que generan las migraciones del sistema.

```bash
php artisan db:generar
php artisan migrate
```

Si trabajas con una base existente, revisa también:

```bash
php artisan db:sincronizar
```

## Crear administrador

```bash
php artisan admin:crear
```

El comando solicita usuario, nombre, correo, DNI y contraseña.

## Ejecutar API

```bash
php artisan serve
```

Por defecto:

```text
http://127.0.0.1:8000
```

## API principal

Las rutas están en:

```text
routes/api.php
```

Se utilizan:

- Sanctum para la autenticación principal.
- Middleware de roles.
- Middleware de auditoría.
- JWT como módulo académico independiente.

## Módulos

Clientes, membresías, pagos, entrenadores, clases, rutinas, asistencias, reservas, categorías, productos, proveedores, compras, ventas, Kardex, caja, usuarios, reportes y auditoría.

## Pruebas

```bash
php artisan test
```

También existen pruebas unitarias para JWT y pruebas básicas de seguridad.
>>>>>>> 67c212c22a11ba7ceb65b36bf231372ef27404ca
