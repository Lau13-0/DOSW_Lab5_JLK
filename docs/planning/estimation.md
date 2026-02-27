# Parte 4 - Estimación del Backlog (Bankify)

## 1. Objetivo

Definir la estimación de historias de usuario y tareas técnicas del backlog inicial de Bankify para planear la primera iteración de desarrollo.

## 2. Técnica de estimación

- **Método:** Planning Poker.
- **Escala:** Serie Fibonacci (`1, 2, 3, 5, 8, 13`).
- **Unidad:** Puntos de historia para HUs y puntos técnicos para tareas.
- **Criterios considerados:** complejidad funcional, riesgo técnico, validaciones, pruebas y dependencias.

## 3. Participantes

- Product Owner (PO): priorización funcional del backlog.
- Scrum Master (SM): facilitación y consolidación de consenso.
- Equipo de Desarrollo: estimación técnica de historias y tareas.

## 4. Estimación de Historias de Usuario

| ID | Historia de Usuario | Estimación (SP) | Justificación breve |
|----|----------------------|-----------------|---------------------|
| HU-01 | Crear nuevo usuario desde administrador | 5 | Requiere modelo, validaciones y endpoint de creación. |
| HU-02 | Autenticar usuario con credenciales | 8 | Implica seguridad, control de sesión y validaciones de acceso. |
| HU-03 | Gestionar estado de cuentas de usuario | 5 | Cambio de estado con reglas de negocio y auditoría básica. |
| HU-04 | Registrar y consultar clientes bancarios | 5 | Incluye alta de datos y consulta con filtros básicos. |

**Total estimado de historias:** `23 SP`.

## 5. Estimación de Tareas Técnicas

| ID | Tarea | HU asociada | Estimación (PT) |
|----|-------|-------------|-----------------|
| TR-01 | Diseñar modelo de datos de usuario | HU-01 | 2 |
| TR-02 | Implementar servicio de creación de usuarios | HU-01 | 3 |
| TR-09 | Crear pruebas unitarias para creación de usuarios | HU-01 | 2 |
| TR-03 | Implementar servicio de autenticación | HU-02 | 5 |
| TR-04 | Crear interfaz de login | HU-02 | 3 |
| TR-10 | Crear pruebas unitarias para autenticación | HU-02 | 2 |
| TR-05 | Implementar funciones de activación/inactivación | HU-03 | 3 |
| TR-06 | Crear interfaz de administración de usuarios | HU-03 | 3 |
| TR-11 | Crear pruebas unitarias para activación/inactivación | HU-03 | 2 |
| TR-07 | Diseñar modelo de datos de clientes | HU-04 | 2 |
| TR-08 | Implementar servicio CRUD de clientes | HU-04 | 5 |
| TR-12 | Crear interfaz de consulta de clientes | HU-04 | 3 |

**Total estimado de tareas técnicas:** `35 PT`.

## 6. Propuesta de distribución por sprint

Suponiendo una capacidad inicial de **12 a 15 SP por sprint**:

- **Sprint 1 (13 SP):** HU-01 (5 SP) + HU-03 (5 SP) + tareas base de pruebas/transversales.
- **Sprint 2 (10 SP):** HU-02 (8 SP) + ajustes de seguridad y hardening.
- **Sprint 3 (5 SP):** HU-04 (5 SP) + estabilización funcional.

> Esta distribución es inicial y debe recalibrarse con la velocidad real del equipo al cierre del Sprint 1.

## 7. Riesgos que pueden afectar estimación

- Cambios de alcance en autenticación y permisos.
- Definición tardía de reglas de validación de datos de clientes.
- Dependencias técnicas no resueltas para UI/API en paralelo.

## 8. Resultado

La parte de estimación queda documentada con una base cuantitativa (`SP` y `PT`) para planear iteraciones, priorizar entregas y dar seguimiento de avance del backlog inicial de Bankify.
