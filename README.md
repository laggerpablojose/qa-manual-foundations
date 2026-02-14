# QA Manual Foundations

Repositorio de práctica profesional orientada a QA Manual (Junior).
Incluye diseño de casos de prueba, reporte de bugs, estrategia básica y evidencia.

## Objetivo 
Construir un portafolio verificable con:
- Test cases claros, reproducibles y trazables.
- Bug reports con severidad, prioridad, entorno y pasos.
- Aplicación de técnicas: Positivo/Negativo, Boundary Value Analysis, Equivalence Partitioning, Smoke y Regression.

## Estructura del repo
- `docs/` -> documentación (glosario, estrategia, entorno)
- `test-cases/` -> casos de prueba por funcionalidad (login, signup, etc.)
- `bug-reports` -> plantilla y reportes de ejemplo
- `evidence/` -> capturas/videos/logs (con guía de nombrado)

## Convenciones

### IDs
- Test Cases: `TC-<FEATURE>-###` (ej: `TC-LOGIN-001`)
- Bugs: `BUG-<FEATURE>-###` (ej: `BUG-LOGIN-001`)

### Severidad (impacot)
- `S1` Crítica: bloqueo total / pérdida de datos / seguridad
- `S2` Alta: funcionalidad principal afectada sin workaround
- `S3` Media: afecta flujo secundario o tiene workaround
- `S4` Baja: visual, texto, detalles menores

### Prioridad (urgencia)
- `P1` Urgente
- `P2` Alta
- `P3` Media
- `P4` Baja

### Contenido inicial (Semana 1)
- Login:
    - Test cases (positivo/negativo/borde)
    - Datos de prueba
    - Bug reports simulados (con pasos reproducibles)

## Cómo usar este repo
1. Ir a `test-cases/login/test-cases-login.md`
2. Ejecutar mentalemnte los escenarios (simulación) o contra una web demo definida en `docs/environment.md`

## Próximos pasos
- Agregar testing sobre Signup y recuperación de contraseña
- Incluir API testing (Postman) en una etapa posterior
- Agregar matriz de trazabilidad simple (requisito -> casos)

---
Autor: Pablo José Lagger