# DOSW_Lab5_JLK

## Parte 4 - Estimación del Backlog (Bankify)

### 1. Objetivo

Definir la estimación de historias de usuario y tareas técnicas del backlog inicial de Bankify para planear la primera iteración de desarrollo.

### 2. Técnica de estimación

- **Método:** Planning Poker.
- **Escala:** Serie Fibonacci (`1, 2, 3, 5, 8, 13`).
- **Unidad:** Puntos de historia para HUs y puntos técnicos para tareas.
- **Criterios considerados:** complejidad funcional, riesgo técnico, validaciones, pruebas y dependencias.

### 3. Participantes

- Product Owner (PO): priorización funcional del backlog.
- Scrum Master (SM): facilitación y consolidación de consenso.
- Equipo de Desarrollo: estimación técnica de historias y tareas.

### 4. Estimación de Historias de Usuario

| ID | Historia de Usuario | Estimación (SP) | Justificación breve |
|----|----------------------|-----------------|---------------------|
| LJK-3 | Creación de cuentas bancarias | 8 | Incluye validación de formato de cuenta, banco asociado y estado de activación. |
| LJK-4 | Consulta de saldo de cuenta | 5 | Requiere validación de pertenencia de cuenta y consulta confiable del saldo. |
| LJK-5 | Realizar depósitos a una cuenta | 5 | Implica validación de monto, actualización de saldo y registro de transacción. |
| LJK-6 | Generación de reporte tributario en PDF | 8 | Tiene mayor complejidad por integración con servicio de generación de reportes. |

**Total estimado de historias:** `26 SP`.

### 5. Estimación de Tareas Técnicas

| ID | Tarea | HU asociada | Estimación |
|----|-------|-------------|------------|
| TR-01 | Diseñar modelo de datos de cuentas bancarias | LJK-3 | 3 |
| TR-02 | Implementar servicio de creación y activación de cuentas | LJK-3 | 5 |
| TR-03 | Crear pruebas unitarias para creación de cuentas | LJK-3 | 2 |
| TR-04 | Implementar servicio de consulta de saldo | LJK-4 | 3 |
| TR-05 | Crear endpoint/controlador de consulta de saldo | LJK-4 | 2 |
| TR-06 | Crear pruebas unitarias para consulta de saldo | LJK-4 | 2 |
| TR-07 | Implementar servicio de depósitos y validación de monto | LJK-5 | 5 |
| TR-08 | Registrar transacciones de depósito | LJK-5 | 3 |
| TR-09 | Crear pruebas unitarias para depósitos | LJK-5 | 2 |
| TR-10 | Implementar generador de reporte tributario PDF | LJK-6 | 5 |
| TR-11 | Integrar servicio externo para exportación de reporte PDF | LJK-6 | 3 |
| TR-12 | Crear pruebas unitarias para generación de reporte PDF | LJK-6 | 2 |

**Total estimado de tareas técnicas:** `37 PT`.

### 6. Propuesta de distribución por sprint

Suponiendo una velocidad de equipo de **20 SP por sprint**:

- Apache Software Foundation. (s.f.). Maven Archetype Plugin. Recuperado el 14 de febrero de 2026, de https://maven.apache.org/archetype/maven-archetype-plugin/
- Apache Software Foundation. (s.f.). maven-archetype-quickstart. Recuperado el 14 de febrero de 2026, de https://maven.apache.org/archetypes/maven-archetype-quickstart/
- GitHub, Inc. (s.f.). About pull requests. Recuperado el 14 de febrero de 2026, de https://docs.github.com/en/pull-requests
- GitHub, Inc. (s.f.). Creating a pull request. Recuperado el 14 de febrero de 2026, de https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/creating-a-pull-request
- GitHub, Inc. (s.f.). Reviewing changes in a pull request. Recuperado el 14 de febrero de 2026, de https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests


## 2. Roles del Equipo Scrum

Los integrantes del equipo han sido asignados a los siguientes roles del marco Scrum:

- **Product Owner**: Laura Castillo - Responsable de definir y priorizar los requisitos del producto.
- **Scrum Master**: Kevin Cuitivaa - Facilita el proceso Scrum y elimina impedimentos para el equipo.
- **Desarrollador**: Juan Silva - Responsable de desarrollar e implementar las funcionalidades del producto.
- **Sprint 1 (18 SP):** LJK-3 (8 SP) + LJK-4 (5 SP) + LJK-5 (5 SP).
- **Sprint 2 (8 SP):** LJK-6 (8 SP) + estabilización funcional.

### 7. Riesgos que pueden afectar estimación

- Cambios de alcance en reglas de validación de cuentas y bancos.
- Definición tardía de políticas para depósitos (límites, controles y auditoría).
- Dependencia externa del servicio de generación de PDF para reportes tributarios.
