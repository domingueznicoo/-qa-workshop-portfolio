Sesión 1

Charter
Explorar si el carrito actualiza correctamente el total al agregar o modificar productos, identificando inconsistencias en montos o pérdida de productos.

ÁREAS
Carrito de compras, Catálogo de productos

INICIO
2026-04-09 19:30
30 minutos

TESTER
Nicolas Dominguez

DESGLOSE DE TAREAS
Navegación y selección de productos: 10 minutos
Pruebas de agregado/modificación en carrito: 10 minutos
Validación de totales y comportamiento: 10 minutos

ARCHIVOS DE DATOS
Productos del catálogo, animales disponibles en la tienda
Cantidades variadas (1, 2, 5, 10) 

NOTAS DE PRUEBA
Se exploró el flujo completo desde la selección de productos hasta la visualización del carrito.
Al agregar múltiples productos, se observó que el total no se actualiza automáticamente, requiriendo presionar el botón “update” para reflejar el monto correcto.

Se probaron distintos escenarios:
Agregar productos distintos
Modificar cantidades
Navegar entre páginas y volver al carrito

Se detectó que el sistema depende de una acción manual para recalcular el total, lo cual no es consistente con una experiencia moderna de e-commerce.

LISTA DE RIESGOS
El sistema podría mostrar montos incorrectos si el usuario no actualiza manualmente el carrito
El usuario podría confiar en un total incorrecto y tomar decisiones de compra equivocadas
Posible abandono del carrito por falta de claridad en el monto final

DEFECTOS (BUGS)
El total del carrito no se actualiza automáticamente al agregar o modificar productos
Dependencia del botón “update” para reflejar cambios en el monto

INCIDENTES (ISSUES)
No está claro si el comportamiento del botón “update” es intencional o un defecto
No hay indicación visual que obligue al usuario a actualizar el carrito

*******************
Sesión 2
Charter

Explorar si el campo de cantidad o campos numéricos aceptan únicamente valores numéricos, identificando comportamientos ante el ingreso de caracteres inválidos (letras, símbolos o valores negativos).

ÁREAS
Carrito de compras, Validación de inputs

INICIO
2026-04-09 20:00
30 minutos

TESTER
Nicolas Dominguez

DESGLOSE DE TAREAS
Identificación de campos numéricos: 10 minutos
Pruebas con datos inválidos: 10 minutos
Validación de comportamiento del sistema: 10 minutos

ARCHIVOS DE DATOS
Valores numéricos válidos: 1, 2, 10
Valores inválidos: "abc", "@#", "-5", "1.5", "" (vacío)

NOTAS DE PRUEBA
Se exploró el campo de cantidad dentro del carrito de compras, probando distintos tipos de entrada.
Se ingresaron valores no numéricos como letras y símbolos, observándose que el sistema permite su ingreso sin validación inmediata.
También se probaron valores negativos y decimales, detectando comportamientos inconsistentes en el procesamiento de la cantidad.
En algunos casos, el sistema no muestra mensajes de error claros ni bloquea la acción, permitiendo avanzar con datos inválidos.

LISTA DE RIESGOS
El sistema podría procesar cantidades inválidas generando errores en el carrito
Posible inconsistencia en cálculos de totales
Falta de validación puede permitir comportamientos inesperados o fallos en el sistema

DEFECTOS (BUGS)
El campo de cantidad permite ingresar caracteres no numéricos
No existen validaciones claras para valores negativos o decimales
El sistema no muestra mensajes de error adecuados ante entradas inválidas

INCIDENTES (ISSUES)
No está definido el comportamiento esperado para valores decimales o negativos
No se especifican reglas claras de validación en la interfaz