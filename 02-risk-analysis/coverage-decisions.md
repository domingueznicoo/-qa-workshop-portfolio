Riesgos que se probarán primero
1.El sistema podría mostrar un total incorrecto en el carrito cuando el usuario agrega un nuevo producto y el monto no se actualiza automáticamente
2.El sistema podría no guardar correctamente la nueva contraseña cuando el usuario la modifica desde “My Account”, impidiendo el acceso posterior
3.El sistema podría permitir completar el checkout con datos inválidos o incompletos

----

¿Por qué esos riesgos son prioridad?
Estos riesgos se priorizan porque impactan directamente en los procesos críticos del negocio y la experiencia del usuario.

En primer lugar, el cálculo incorrecto del total en el carrito afecta directamente la transacción principal del sistema, pudiendo generar cobros erróneos o pérdida de ventas, lo que representa un impacto alto tanto para el negocio como para el usuario.

En segundo lugar, la falla en la actualización de contraseña compromete el acceso del usuario a su cuenta, lo que afecta la confianza en el sistema y puede generar bloqueos o abandono de la plataforma.

Por último, permitir completar el checkout con datos inválidos puede derivar en pedidos incorrectos, fallos en la entrega o problemas en el procesamiento de pagos, impactando la operación del negocio y generando reclamos.

En conjunto, estos riesgos están directamente relacionados con funcionalidades críticas: compra, autenticación y validación de datos, por lo que deben ser abordados en las primeras etapas del testing.

----

Qué se probará menos o quedará fuera por ahora
-Validación de ingreso de valores no numéricos en el campo de cantidad
-Inconsistencias en imágenes del catálogo o buscador
-Comportamientos secundarios de navegación (búsqueda y visualización de productos)

----

Justificación de exclusiones

Estos elementos se consideran de menor prioridad en una primera fase de testing porque su impacto en el negocio es menor en comparación con los riesgos críticos.

La validación de campos, aunque importante, generalmente es manejada por controles básicos y no afecta directamente la transacción principal si el sistema falla de forma controlada.

Las inconsistencias en imágenes del catálogo afectan principalmente la experiencia visual del usuario, pero no impiden la compra ni generan pérdidas directas para el negocio.

Por último, los aspectos relacionados a navegación o búsqueda tienen un impacto más orientado a usabilidad que a funcionamiento crítico, por lo que pueden ser evaluados en una etapa posterior.

Esta priorización permite enfocar los esfuerzos de testing en las funcionalidades que representan mayor riesgo para el negocio, optimizando el uso del tiempo y recursos disponibles.