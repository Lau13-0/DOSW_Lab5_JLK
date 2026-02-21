# Planeación del Sistema Bankify

## Desglose de trabajo: Épicas, Historias de Usuario y Tareas

La implementación de los requerimientos identificados de Bankify se desglose de la siguiente manera:

---

## 1. Épicas:

| Campo | Descripción |
|-------|-------------|
| **ID** | EP-01 |
| **Título** | Autenticación y Gestión de Usuarios |
| **Descripción** | Bankify necesita esta épica para establecer un sistema seguro de autenticación que permita a operadores y clientes acceder a la plataforma con credenciales de usuario y contraseña. Además, es necesario un módulo de gestión de usuarios que permita a los administradores crear, activar e inactivar cuentas de usuario de forma controlada. |
| **Stakeholder** | Administradores del sistema, Operadores de Bankify y Clientes finales |

---

## 2. Historias de Usuario:

| Campo | Descripción |
|-------|-------------|
| **ID** | HU-01 |
| **Título** | Crear nuevo usuario desde administrador |
| **Descripción** | Como administrador del sistema quiero crear nuevas cuentas de usuario con nombre de usuario y contraseña para que operadores y clientes puedan acceder a la plataforma Bankify |
| **Épica asociada** | EP-01 |

| Campo | Descripción |
|-------|-------------|
| **ID** | HU-02 |
| **Título** | Autenticar usuario con credenciales |
| **Descripción** | Como usuario (operador o cliente) quiero iniciar sesión con mi usuario y contraseña para acceder a mis funcionalidades en la plataforma |
| **Épica asociada** | EP-01 |

| Campo | Descripción |
|-------|-------------|
| **ID** | HU-03 |
| **Título** | Gestionar estado de cuentas de usuario |
| **Descripción** | Como administrador quiero activar e inactivar cuentas de usuario para controlar el acceso a la plataforma |
| **Épica asociada** | EP-01 |

| Campo | Descripción |
|-------|-------------|
| **ID** | HU-04 |
| **Título** | Registrar y consultar clientes bancarios |
| **Descripción** | Como administrador quiero crear y consultar información de clientes para gestionar los datos de quiénes son los titulares de las cuentas bancarias |
| **Épica asociada** | EP-02 |

---

## 3. Tareas:

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-01 |
| **Título** | Diseñar modelo de datos de usuario |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Crear el modelo de datos para almacenar información de usuarios (username, contraseña hasheada, estado, tipo de rol) |
| **Tareas requisito** | Ninguna |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-02 |
| **Título** | Implementar servicio de creación de usuarios |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Desarrollar la lógica para crear nuevos usuarios con validación de datos (username único, contraseña segura) |
| **Tareas requisito** | TR-01 |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-03 |
| **Título** | Implementar servicio de autenticación |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Desarrollar el servicio de validación de credenciales y generación de sesiones/tokens |
| **Tareas requisito** | TR-01 |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-04 |
| **Título** | Crear interfaz de login |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Desarrollar la interfaz de usuario para que los usuarios inicien sesión |
| **Tareas requisito** | TR-03 |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-05 |
| **Título** | Implementar funciones de activación/inactivación de usuarios |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Desarrollar la lógica para cambiar el estado activo/inactivo de una cuenta de usuario |
| **Tareas requisito** | TR-01 |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-06 |
| **Título** | Crear interfaz de administración de usuarios |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Desarrollar la interfaz para que administradores puedan gestionar (crear, activar, inactivar) usuarios |
| **Tareas requisito** | TR-02, TR-05 |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-07 |
| **Título** | Diseñar modelo de datos de clientes |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Crear el modelo de datos para almacenar información de clientes bancarios |
| **Tareas requisito** | Ninguna |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-08 |
| **Título** | Implementar servicio CRUD de clientes |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Desarrollar los servicios para crear, leer, actualizar y eliminar información de clientes |
| **Tareas requisito** | TR-07 |
