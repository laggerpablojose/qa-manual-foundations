# 📘 QA FUNDAMENTOS – SEMANA 1

---

# 1 ¿Qué es QA?

## Definición profesional

**QA (Quality Assurance)** es el proceso mediante el cual se asegura que un producto cumple con los requisitos definidos y funciona correctamente antes de llegar al usuario final.

No es solo “buscar errores”.

Es:

* Verificar requisitos.
* Detectar inconsistencias.
* Validar reglas de negocio.
* Documentar defectos.
* Reducir riesgos.

---

# 2 QA vs QC (Concepto clave de entrevista)

| QA             | QC               |
| -------------- | ---------------- |
| Proceso        | Producto         |
| Preventivo     | Detectivo        |
| Mejora calidad | Detecta defectos |

QA trabaja en el proceso.
QC inspecciona el resultado.

En equipos pequeños, el QA hace ambos.

---

# 3 ¿Qué hace un QA Manual en la práctica?

Un QA manual:

* Lee especificaciones.
* Diseña test cases.
* Ejecuta pruebas manuales.
* Reporta bugs.
* Valida correcciones.
* Participa en sprint planning.
* Hace regression testing.

No programa.
Pero debe entender lógica.

---

# 4 Tipos de Testing (Fundamentales)

---

## 🔹 Testing Funcional

Valida que el sistema haga lo que debe hacer.

Ejemplo:
Login redirige al dashboard.

---

## 🔹 Testing No Funcional

Evalúa aspectos como:

* Performance
* Seguridad
* Usabilidad
* Compatibilidad

Ejemplo:
La app carga en menos de 3 segundos.

---

## 🔹 Testing Positivo

Se prueba con datos correctos.

Ejemplo:
Email válido + password válida → acceso permitido.

---

## 🔹 Testing Negativo

Se prueba con datos incorrectos.

Ejemplo:
Email inválido → error mostrado.

---

## 🔹 Boundary Value Analysis (BVA)

Técnica para probar valores límite.

Si mínimo es 8:

* 7
* 8
* 9

Es técnica obligatoria en QA.

---

## 🔹 Equivalence Partitioning

Se dividen datos en grupos equivalentes.

Ejemplo edad 18–60:

Grupo válido:

* 18–60

Grupo inválido:

* "<"18
* ">" 60
* Letras
* Vacío

No se prueban todos los números.
Se prueba uno representativo de cada grupo.

---

## 🔹 Smoke Testing

Prueba rápida para verificar que lo principal funciona.

Ejemplo:
La app abre.
Login funciona.
Se puede navegar.

---

## 🔹 Regression Testing

Se prueba nuevamente algo que ya funcionaba para verificar que no se rompió tras un cambio.

Muy común en cada sprint.

---

# 5 Test Case Profesional

Documento que define cómo probar algo.

Estructura estándar:

* ID
* Título
* Precondición
* Pasos
* Resultado esperado
* Tipo

Debe ser:

* Claro
* Reproducible
* No ambiguo
* Basado en requisitos

---

# 6 Bug Report Profesional

Un bug no es:

“No funciona”.

Un bug debe incluir:

* ID
* Título claro
* Severidad (impacto técnico)
* Prioridad (urgencia negocio)
* Entorno
* Pasos exactos
* Resultado actual
* Resultado esperado
* Evidencia

Ejemplo malo:
“Login no anda”.

Ejemplo profesional:
“Al ingresar password con 7 caracteres el sistema permite acceso, incumpliendo regla de mínimo 8 caracteres”.