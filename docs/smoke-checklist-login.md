## Smoke Test checklist

# Alcance 
- Evaluaremos el software utilizando un conjunto mínimo de pruebas críticas 
- El Objetivo será validar que la funcionalidad crítica del sistema operan correctamente antes de continuar con pruebas más profundas o despliegue.

# Checklist
1. Verificar que la página de login carga correctamente.
2. Verificar que el login con credenciales válidas redirige a Secure Area y muestre mensaje de éxito.
3. Verificar que el Secure Area muestre la infromación correspondiente.
4. Verificar que el logout redirije correctamente al login y muestre mesnaje de éxito.
5. Verificar que no se puede acceder a Secure Area sin iniciar la sesión (acceso directo por URL).
6. Verificar que el bug crítico (Back tras logout) mantiene el comportamiento observado.

# Resultado
- Smoke test aprobado.
- No se detectan bloqueantes para continuar con pruebas adicionales o despliegue. 

capturas:
![Smoke test N1](../evidence/login/login-smoke-test-001)
![Smoke test N2](../evidence/login/login-smoke-test-002)