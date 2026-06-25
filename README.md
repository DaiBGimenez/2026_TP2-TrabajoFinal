# 2026_TP2-TrabajoFinal
Trabajo grupal de la materia Taller de progrmacion 2, Instituto ORT 2026

## Descripción
Este proyecto consiste en una **API REST** desarrollada con **Node.js**, **Express** y **MongoDB**, destinada a administrar los distintos procesos de una aplicación ecommerce

La aplicación implementa una arquitectura por capas para separar responsabilidades y facilitar el mantenimiento del código.

---

# Funcionalidades principales

La API permite administrar:

- Usuarios
    - Registro
    - Inicio de sesión
    - Autenticación mediante JWT

- Productos
    - Alta
    - Baja
    - Modificación
    - Consulta

- Carrito
    - Agregar productos
    - Eliminar productos
    - Consultar carrito

- Pedidos
    - Crear pedidos
    - Consultar pedidos

- Producción
    - Gestión de producción

---

# Listado de Endpoints 

- Productos

| Método | Endpoint | Descripción |
|---------|----------|-------------|
| GET | /api/products/ | Obtener productos |
| GET | /api/products/:id | Obtener producto especifico |
| POST | /api/products/ | Crear producto |
| PUT | /api/products/:id | Actualizar producto |
| DELETE | /api/products/:id | Borrar producto |

- Usuarios

| Método | Endpoint | Descripción |
|---------|----------|-------------|
| GET | /api/users/ | Usuarios |
| GET | /api/users/:id | Usuario especifico |
| PUT | /api/users/:id | Actualizar Usuario |
| POST | /api/users/login | Iniciar sesión |
| POST | /api/users/register | Registrar usuario |
| DELETE | /api/users/:id | Eliminar usuario|

- Carrito

| Método | Endpoint | Descripción |
|---------|----------|-------------|
| GET | /api/cart/ | Obtener carrito |
| POST | /api/cart/add | Agregar al carrito |
| DELETE | /api/cart/remove/:id | Sacar producto del carrito |
| DELETE | /api/cart/clear | Vaciar el carrito |
| POST | /api/cart/checkout | Checkout |

-Pedidos

| Método | Endpoint | Descripción |
|---------|----------|-------------|
| GET | /api/orders/ | Obtener pedidos |
| GET | /api/orders/:id | Obtener pedido especifico |
| PUT | /api/orders/:id | Editar pedido |
| PUT | /api/orders/:id/status | Actualizar pedido |
| PUT | /api/orders/:id/cancel | Cancelar pedido |
| DELETE | /api/orders/:id | Eliminar pedido |

-Produccion

| Método | Endpoint | Descripción |
|---------|----------|-------------|
| GET | /api/production | Producción |

---

# Base de datos

La aplicación utiliza MongoDB para almacenar la información correspondiente a:

- Usuarios
- Productos
- Carritos
- Pedidos
- Producción
