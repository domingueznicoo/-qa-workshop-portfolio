# Risk Matrix

| ID | Riesgo | Impacto | Probabilidad | Nivel | Justificación |
|----|--------|---------|--------------|-------|---------------|
| R1 | El sistema podría mostrar un total incorrecto en el carrito cuando el usuario agrega un nuevo producto y el monto no se actualiza automáticamente | 5 | 4 | 20 | Afecta directamente la experiencia de compra y puede generar confusión, errores en el pago o abandono del carrito |
| R2 | El sistema podría no guardar correctamente la nueva contraseña cuando el usuario la modifica desde “My Account”, impidiendo el acceso posterior con las credenciales actualizadas | 5 | 4 | 20 | Impacta el acceso a la cuenta y la confianza del usuario, ya que la operación parece realizarse pero luego falla el inicio de sesión |
| R3 | El sistema podría permitir ingresar valores no numéricos en el campo de cantidad antes de confirmar la compra | 3 | 4 | 12 | Es una falla de validación que puede afectar cálculos, cantidades y estabilidad del flujo de compra |
| R4 | El sistema podría permitir completar el checkout con datos inválidos o incompletos, como dirección o información de pago inconsistente | 5 | 3 | 15 | Puede provocar errores operativos, fallos en pedidos y mala experiencia del cliente |
| R5 | El catálogo o buscador podría mostrar imágenes incorrectas para los animales, no coincidiendo con el nombre del producto | 3 | 4 | 12 | Genera confusión, afecta la confianza del usuario y deteriora la calidad percibida del sistema |