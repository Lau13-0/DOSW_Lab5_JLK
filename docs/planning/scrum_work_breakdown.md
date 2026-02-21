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
| **Prioridad** | Alta |
| **Estimación** | 5 puntos - Funcionalidad foundacional que requiere diseño del modelo de datos y servicio REST. Complejidad media por validaciones y gestión de contraseñas. |
| **Épica asociada** | EP-01 |

| Campo | Descripción |
|-------|-------------|
| **ID** | HU-02 |
| **Título** | Autenticar usuario con credenciales |
| **Descripción** | Como usuario (operador o cliente) quiero iniciar sesión con mi usuario y contraseña para acceder a mis funcionalidades en la plataforma |
| **Prioridad** | Alta |
| **Estimación** | 8 puntos - Funcionalidad crítica que requiere implementar autenticación segura, gestión de sesiones y tokens JWT. Complejidad alta por requerimientos de seguridad. |
| **Épica asociada** | EP-01 |

| Campo | Descripción |
|-------|-------------|
| **ID** | HU-03 |
| **Título** | Gestionar estado de cuentas de usuario |
| **Descripción** | Como administrador quiero activar e inactivar cuentas de usuario para controlar el acceso a la plataforma |
| **Prioridad** | Media |
| **Estimación** | 5 puntos - Funcionalidad de apoyo para administración. Complejidad media por manejo de estados y auditoría de cambios de estado. |
| **Épica asociada** | EP-01 |

| Campo | Descripción |
|-------|-------------|
| **ID** | HU-04 |
| **Título** | Registrar y consultar clientes bancarios |
| **Descripción** | Como administrador quiero crear y consultar información de clientes para gestionar los datos de quiénes son los titulares de las cuentas bancarias |
| **Prioridad** | Alta |
| **Estimación** | 5 puntos - Funcionalidad crítica para negocio. Complejidad media por captura de datos complejos y búsqueda/filtrado de información de clientes. |
| **Épica asociada** | EP-02 |

---

## 3. Tareas:

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-01 |
| **Título** | Diseñar modelo de datos de usuario |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Como desarrollador quiero diseñar el modelo de datos de usuario para almacenar información de usuarios de forma estructurada |
| **Tareas requisito** | Ninguna |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-02 |
| **Título** | Implementar servicio de creación de usuarios |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Como desarrollador quiero implementar el servicio de creación de usuarios para permitir que los administradores registren nuevas cuentas |
| **Tareas requisito** | TR-01 |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-03 |
| **Título** | Implementar servicio de autenticación |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Como desarrollador quiero implementar el servicio de autenticación para validar credenciales y generar sesiones |
| **Tareas requisito** | TR-01 |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-04 |
| **Título** | Crear interfaz de login |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Como desarrollador quiero crear la interfaz de login para que los usuarios puedan iniciar sesión en la plataforma |
| **Tareas requisito** | TR-03 |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-05 |
| **Título** | Implementar funciones de activación/inactivación de usuarios |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Como desarrollador quiero implementar las funciones de activación/inactivación para permitir controlar el acceso de usuarios |
| **Tareas requisito** | TR-01 |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-06 |
| **Título** | Crear interfaz de administración de usuarios |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Como desarrollador quiero crear la interfaz de administración para que los administradores gestionen cuentas de usuario |
| **Tareas requisito** | TR-02, TR-05 |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-07 |
| **Título** | Diseñar modelo de datos de clientes |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Como desarrollador quiero diseñar el modelo de datos de clientes para almacenar información de titulares de cuentas |
| **Tareas requisito** | Ninguna |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-09 |
| **Título** | Crear pruebas unitarias para creación de usuarios |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Como desarrollador quiero crear pruebas unitarias para validar la funcionalidad de creación de usuarios |
| **Tareas requisito** | TR-02 |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-10 |
| **Título** | Crear pruebas unitarias para autenticación |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Como desarrollador quiero crear pruebas unitarias para validar la funcionalidad de autenticación |
| **Tareas requisito** | TR-03 |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-11 |
| **Título** | Crear pruebas unitarias para activación/inactivación de usuarios |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Como desarrollador quiero crear pruebas unitarias para validar el cambio de estado de cuentas de usuario |
| **Tareas requisito** | TR-05 |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-12 |
| **Título** | Crear interfaz de consulta de clientes |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Como desarrollador quiero crear la interfaz de consulta para que administradores puedan visualizar información de clientes |
| **Tareas requisito** | TR-08 |

| Campo | Descripción |
|-------|-------------|
| **ID** | TR-08 |
| **Título** | Implementar servicio CRUD de clientes |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Como desarrollador quiero implementar el servicio CRUD de clientes para permitir gestionar información de clientes |
| **Tareas requisito** | TR-07 |
