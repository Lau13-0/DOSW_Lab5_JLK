# DOSW_Lab4_JLK

a. ¿Qué es un arquetipo (Archetype) en Maven?

Un arquetipo en Maven es una plantilla o mecanismo de generación de proyectos que permite crear la estructura inicial de un proyecto (directorios, archivos y un `pom.xml` básico) siguiendo un patrón predefinido. Los arquetipos facilitan la estandarización y el inicio rápido de nuevos proyectos.

b. ¿Para qué sirve el arquetipo `maven-archetype-quickstart`?

El arquetipo `maven-archetype-quickstart` sirve para generar un proyecto Java simple y listo para compilar, que incluye la estructura de directorios (`src/main/java`, `src/test/java`), un `pom.xml` mínimo, una clase de ejemplo y una clase de prueba. Es útil para iniciar rápidamente proyectos Java de tipo aplicación o librería con una configuración básica.

c. ¿Cuál es el comando con el cual se puede crear un proyecto basado en un arquetipo maven?

Ejemplo de comando para crear un proyecto usando `maven-archetype-quickstart` (no interactivo):

```
mvn archetype:generate -DgroupId=com.ejemplo -DartifactId=mi-proyecto -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
```

Este comando genera un nuevo proyecto con `groupId` y `artifactId` especificados usando el arquetipo indicado. Si se omiten parámetros, Maven puede entrar en modo interactivo para seleccionar opciones.

d. ¿Qué es un pull request en GitHub?

Un pull request (PR) en GitHub es una solicitud para fusionar (merge) cambios realizados en una rama (o fork) hacia otra rama del repositorio (por ejemplo, `feature-branch` → `main`). El PR permite revisión de código, discusión, comprobaciones automáticas (CI) y aprobación antes de integrar los cambios.

e. ¿Cómo se crea un pull request en GitHub?

1. Crear y commitear los cambios en una nueva rama local y subirla al repositorio remoto (`git push origin mi-rama`).
2. En la interfaz web de GitHub, ir al repositorio y seleccionar la opción "Compare & pull request" o "New pull request".
3. Elegir la rama origen y destino, añadir título y descripción, asignar revisores y etiquetas si procede.
4. Hacer clic en "Create pull request" para abrir el PR.

f. ¿Cómo se aprueba un pull request en GitHub?

Un revisor abre el PR, examina los cambios y puede dejar comentarios. Para aprobarlo, el revisor selecciona "Review changes" y elige la opción "Approve". Tras las aprobaciones y una vez que las comprobaciones (checks) obligatorias pasan, alguien con permisos puede fusionar el PR usando "Merge pull request" (o las opciones "Squash and merge" / "Rebase and merge"). En organizaciones con políticas de protección de ramas, puede ser necesario un número mínimo de aprobaciones y que los checks de CI estén verdes.

g. Bibliografía (norma APA)

- Apache Software Foundation. (s.f.). Maven Archetype Plugin. Recuperado el 14 de febrero de 2026, de https://maven.apache.org/archetype/maven-archetype-plugin/
- Apache Software Foundation. (s.f.). maven-archetype-quickstart. Recuperado el 14 de febrero de 2026, de https://maven.apache.org/archetypes/maven-archetype-quickstart/
- GitHub, Inc. (s.f.). About pull requests. Recuperado el 14 de febrero de 2026, de https://docs.github.com/en/pull-requests
- GitHub, Inc. (s.f.). Creating a pull request. Recuperado el 14 de febrero de 2026, de https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/creating-a-pull-request
- GitHub, Inc. (s.f.). Reviewing changes in a pull request. Recuperado el 14 de febrero de 2026, de https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests
