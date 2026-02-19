# Test Cases - Login (The Internet)

SUT: The Internet - From Authentication
Feature: Login/Logout
Técnica: Positivo/Negativo, BVA (mínimos), validaciones básicas.

## Formato
- **ID:**
- **Título:**
- **Precondición:**
- **Datos de prueba:**
- **Pasos:**
- **Resultado esperado:**
- **Tipo:** (Positiva/Negativa/Borde)

- **ID:** TC-LOGIN-001
- **Título:** 
Prueba de login exitoso con credenciales válidas 
- **Precondición:** 
Usuario en pantalla de login.
- **Datos de prueba:** 
Username: "tomsmith" 
Password: "SuperSecretPassword!"
- **Pasos:**
1. Ingreso Username: "tomsmith"
2. Ingreso Password: "SuperSecretPassword!"
3. Presiono button "Login"
- **Resultado esperado:** 
El sistema redirige a la página segura. 
Se visualiza mensaje de éxito: "You logged into a secure area!".
- **Tipo:** Positiva

--- 

- **ID:** TC-LOGIN-002
- **Título:** 
Test de logout exitoso desde área seguro
- **Precondición:** 
Usuario previamente logueado. Ubicado en Secure Area.
- **Datos de prueba:**
Username: "tomsmith" 
Password: "PasswordIncorrecta!"
- **Pasos:**
1. Presiono button "Logout"
- **Resultado esperado:** 
Logout exitoso. 
Mensaje de cierre de sesión exitoso: "You logged out of the secure area!". 
El sistema ubica al usuario en pantalla de login.
- **Tipo:** Positiva

---

- **ID:** TC-LOGIN-003
- **Título:** 
Prueba de password incorrecta con username válido.
- **Precondición:**
Usuario en pantalla de login.
- **Datos de prueba:** 
Username: "tomsmith" 
Password: "PasswordIncorrecta!"
- **Pasos:**
1. Ingreso Username: "tomsmith"
2. Ingreso Password: "PasswordIncorrecta!"
3. Presiono button "Login"
- **Resultado esperado:** 
Login NO aceptado.
Mensaje de credenciales inválidas.
- **Tipo:** Negativa

---

- **ID:** TC-LOGIN-004
- **Título:** 
Prueba de username incorrecto con password válida
- **Precondición:**
Usuario en pantalla de login.
- **Datos de prueba:** 
Username: "smitetomas" 
Password: "SuperSecretPassword!"
- **Pasos:**
1. Ingreso username inválido: "smitetomas"
2. Ingreso password válida: "SuperSecretPassword!"
3. Presiono button "Login"
- **Resultado esperado:** 
Login rechazado.
Mensaje al usuario: "Your username is invalid!"
- **Tipo:** Negativa

---

- **ID:** TC-LOGIN-005
- **Título:** 
Prueba de username y password incorrectos
- **Precondición:** 
Usuario en pantalla de login.
- **Datos de prueba:** 
Username: "smitetomas"
Password: "PasswordIncorrecta!"
- **Pasos:**
1. Ingreso username inválido: "smitetomas"
2. Ingreso password inválida: "PasswordIncorrecta!"
3. Presiono button "Login"
- **Resultado esperado:** 
Login rechazado. 
Mensaje de credenciales incorrectas: "Your username is invalid!".
Acceso a Secure area denegado.
- **Tipo:** Negativa

---

- **ID:** TC-LOGIN-006
- **Título:** 
Prueba de Username vacío.
- **Precondición:** 
Usuario en pantalla de login.
- **Datos de prueba:** 
Username: "" 
Password: "SuperSecretPassword!"
- **Pasos:**
1. Ingreso Username vacío: ""
2. Ingreso Password: "SuperSecretPassword!"
3. Presiono button "Login"
- **Resultado esperado:**
Login rechazado. 
El sistema no permite acceder a la información protegida.
Mensaje de credenciales rechazadas: "Your username is invalid!".
- **Tipo:** Negativa

---

- **ID:** TC-LOGIN-007
- **Título:** 
Prueba de password vacío 
- **Precondición:** 
Usuario en pantalla de login.
- **Datos de prueba:** 
Username: "tomsmith"
Password: ""
- **Pasos:**
1. Ingreso Username: "tomsmith".
2. Ingreso Password vacía: "".
3. Presiono button "Login"
- **Resultado esperado:**
Login rechazado. 
Mensaje: "Your password is invalid!"
- **Tipo:** Negativa

---

- **ID:** TC-LOGIN-008
- **Título:** 
Username con espacio adelante/atrás
- **Precondición:** 
Usuario en pantalla de login.
- **Datos de prueba:** 
Username: " tomsmith "
Password: "SuperSecretPassword!"
- **Pasos:**
1. Ingreso Username con espacio al inicio y fin: " tomsmith "
2. Ingreso Pasword: "SuperSecretPassword!".
3. Presiono button "Login"
- **Resultado esperado:** 
Losing rechazado
Mensaje de credenciales inválida: "Your username is invalid!".
- **Tipo:** Borde / Negativa (según resultado)

---

- **ID:** TC-LOGIN-009
- **Título:** 
Test de password con espacio adelante/atrás.
- **Precondición:** 
Usuario en pantalla de login.
- **Datos de prueba:** Username="tomsmith", password=" SuperSecretPassword! "
- **Pasos:**
1. Ingreso Username: "tomsmith".
2. Ingreso Pasword con espacio al inicio y fin: " SuperSecretPassword! ".
3. Presiono button "Login"
- **Resultado esperado:** 
El sistema no elimina espacio.
Mensaje de credenciales inválidas.
- **Tipo:** Borde / Negativa (según resultado)

---

- **ID:** TC-LOGIN-010
- **Título:** 
Verificar persistencia de sesión al refrescar después de login.
- **Precondición:** 
Usuario en pantalla de login.
- **Datos de prueba:** 
Username: "tomsmith"
Password: "SuperSecretPassword!"
- **Pasos:**
1. Ingreso username válido.
2. Ingreso pasword válido.
3. Presiono button "Login".
4. Refresco la pagina(F5)
- **Resultado esperado:** 
El usuario permance en la Secure Area.
No es redirigido al login.
El contenido protegido sigue visible. 
- **Tipo:** Positiva (gestión de sesion)