# Cómo trabajamos con ramas

## Estrategia
GitHub Flow con ramas cortas. `main` siempre está lista para publicar.
Cuando haya pruebas automáticas suficientes, el objetivo es pasar a trunk-based.

## La aplicación del almacén
Cuando pase a Git, Release Flow: una rama de versión por cada versión que se instala, y los arreglos, primero en `main`.

## Ramas
- Todo el trabajo sale de `main` y vuelve a `main` por pull request.
- Nombre: `users/<usuario>/<número de tarea>-<descripción>`.
- Una rama no debería pasar de tres días abierta.

## Commits
- Un motivo por commit, con el número de la tarea (#123) en el mensaje.
- Formato del mensaje: Conventional Commits (`feat:`, `fix:`), si el equipo lo adopta.

## Rebase y push forzado
- Si alguien más tiene tus commits, merge. Si son solo tuyos, puedes hacer rebase.
- Push forzado solo en tu propia rama, y con lease.

## Versiones
- Cada publicación se marca con una etiqueta anotada: v<mayor>.<menor>.<parche>.

## Pull requests
- Primera revisión, el mismo día.
- La descripción dice qué cambia y por qué, qué mirar con más cuidado, cómo se comprueba y qué no hace.
- Tipo de merge al completar: squash.
- La rama se borra al completar.

## Políticas de `main`
- Lo que aquí se acuerda, las políticas lo hacen cumplir: un revisor como mínimo, que no sea el autor; tarea enlazada; comentarios resueltos, y solo squash.
- Pueden saltarse las políticas al completar, solo en emergencias: Diego e Irene. Cada vez que se use, se cuenta en el canal del equipo.
