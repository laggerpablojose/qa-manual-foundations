# Bug Report

**ID:** BUG-LOGIN-001
**Título:** Tras Logout, el botón "Back" permite visualizar contenido de Secura Area en cache (hasta refrescar)

**Severidad:** S3 
**Prioridad:** P2 

**Entorno:** Windows 11, Chrome (v:145.0.7632.76), The Internet - From Authentication
**Preciondición:** Usuario autenticado en Secure Area

## Pasos para reproducir
1. Ir a la pantalla de login del SUT.
2. Iniciar sesión con credenciales válidas (username: "tomsmith", password: "SuperSecretPassword!").
3. Conformar que se visualiza la página Secure Area.
4. Hacer click en Logout.
5. En la pantalla de login (post logout), presionar el botón Back del navegador.

## Resultado actual
- El navegador vuelve a mostrar la pantalla Secure Area con contenido visible (aparentemente cachead).
- Al referscar la pagina (F5), el sistema redirige a login ("You must login to view the secure area!").

## Resultado esperado
- Luego del logout, al usar BACK, el sistema no debería permitir visualizar contenido protegido.
- El usuario debería ser redirigido al login o mostrarse una pantalla sin información sensible.

## Evidencia
- 