## Matriz de trazabilidad 

# Requisitos funcionales

|Requisito   |Descripción                                                                         |Test cases asociados |Estado    |
|------------|------------------------------------------------------------------------------------|---------------------|----------|
|RF-LOGIN-001|Autenticación válida permite acceso.                                                |TC-LOGIN-001         |Passed    |
|RF-LOGIN-002|Autenticación inválida es rechazada.                                                |TC-LOGIN-003,004,005 |Passed    |
|RF-LOGIN-003|Logout invalida sesión.                                                             |TC-LOGIN-002         |Passed    |
|RF-LOGIN-005|Acceso directo a área segura sin login es bloqueado.                                |TC-LOGIN-010         |Passed    |
|RF-LOGIN-006|El sistema gestiona inputs vacíos correctamente.                                    |TC-LOGIN-006, 007    |Passed    |
|RF-LOGIN-007|El sistema gestiona variaciones de formato (espacios) según comportamiento definido.|TC-LOGIN-008, 009    |Failed    |
