# QA Manual Foundations

Repositorio de práctica profesional orientado a QA Manual (Junior), estructurado por iteraciones versionadas y siguiendo un flujo de trabajo similar a entornos reales (branches, Pull Requests y tags).
Incluye diseño de casos de prueba, reporte formal de defectos, estrategia básica y evidencia documentada.

## Objetivo 
Construir un portafolio verificable que demuestre:
- Test cases claros, reproducibles y trazables.
- Bug reports con severidad, prioridad, entorno y pasos detallados.
- Aplicación de técnicas de pruebas:
    * Positivo/Negativo
    * Boundary Value Analysis
    * Equivalence Partitioning
    * Smoke Testing 
    * Regression Testing

## Versionado
### v0.1-Login QA Pack (Semana 1)
Incluye.
* 10 test cases del módulo Login
* Análisis de equivalencia
* Definición de entorno de pruebas
* Documento de entorno de pruebas
* Smoke test checklist
* Matriz de trazabilidad (Login)
* Bug report documentado con evidencia (capturas + video externo)
Tag: `v0.1`

## Estructura del repo
- `docs/` -> documentación (estrategia, entorno, análisis, matrices)
- `test-cases/` -> casos de prueba por funcionalidad (login, signup, etc.)
- `bug-reports` -> plantilla y reportes de ejemplo
- `evidence/` -> capturas organizadas por módulo (con convención de nombrado)

## Convenciones

### IDs
- Test Cases: `TC-<FEATURE>-###` 
    Ejemplo: `TC-LOGIN-001`
- Bugs: `BUG-<FEATURE>-###`
    Ejemplo: `BUG-LOGIN-001`

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

## Cómo usar este repositorio
1. Revisar los casos en test-cases/login/test-cases-login.md
2. Consultar el entorno en docs/environment.md
3. Ejecutar escenarios contra la web definida en el entorno
4. Ver reportes en bug-reports/ con evidencia asociada

## Metodología de trabajo
* `main` siempre estable
* Trabajo por feature branch
* Pull Requests por iteración
* Versionado mediante tags
* Evidencia asociada a cada defecto documentado

## Próximas iteraciones
* Ampliar cobertura del módulo Login (regresión)
* Agregar módulo Signup
* Agregar recuperación de contraseña
* Incorporar API testing (Postman)
* Preparar base para futura automatización

---
Autor: Pablo José Lagger