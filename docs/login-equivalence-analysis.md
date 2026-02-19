## Campo Username

### Grupo válido:
* Username exacto válido proporcionado por el sistema

### Grupo inválido:
* Username incorrecto (string arbitrario)
* Username vacío o solo espacios
* Username con espacios al inicio, al fin (evaluar trim)
* Username con caracteres unicode/símbolos.
* Username con logitud exesivas (stress input)
* Username con contenido tipo script o URL

## Campo Password

### Grupo válido
* Password exacta válida proporcionada por el sistema

### Grupo inválido
* Password incorrecta (string arbitraria)
* Password vacía o solo espacios
* Password con espacios al inicio, al fin (evaluar trim)
* Password con logitud excesiva (stress input)
* Password con contenido tipo script o URL
* Password con variaciones mínimas (ej: cambio de matúscula)
