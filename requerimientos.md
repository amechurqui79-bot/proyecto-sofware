# Especificación de requerimientos

## Sistema de gestión de pedidos - Pastelería Dulce Tentación

Basado en IEEE 830-1998  
Versión 1.0 · 24 de noviembre de 2026

---

## 1. Introducción

### 1.1 Propósito

Especificar los requerimientos funcionales y no funcionales del sistema de gestión de pedidos para la Pastelería Dulce Tentación, estableciendo las funciones y condiciones que deberá cumplir el sistema para facilitar el registro, almacenamiento, consulta y seguimiento de los pedidos realizados por los clientes.

Los requerimientos servirán como base para el desarrollo y las pruebas del sistema, permitiendo verificar si las funcionalidades implementadas cumplen con las necesidades identificadas en el negocio.

### 1.2 Alcance

El sistema permitirá registrar los pedidos de los clientes, almacenar sus datos en una base de datos, consultar los pedidos pendientes según su fecha de entrega y actualizar su estado cuando hayan sido entregados.

También permitirá consultar los productos disponibles de la pastelería para facilitar la selección durante el registro de un pedido.

El sistema estará destinado principalmente a la propietaria y al personal encargado de atender los pedidos.

No incluye facturación, pagos electrónicos, gestión de inventario de materias primas ni envío automático de notificaciones por WhatsApp o SMS, conforme a los límites establecidos en la propuesta del proyecto.

### 1.3 Definiciones

| Término | Significado en este documento |
|---|---|
| **Pedido** | Encargo realizado por un cliente que contiene uno o más productos y una fecha de entrega. |
| **Cliente** | Persona que solicita uno o varios productos de la pastelería. |
| **Pendiente** | Pedido que todavía no ha sido marcado como entregado. |
| **Entregado** | Pedido que ya fue preparado y entregado al cliente. |
| **Operador** | Persona que utiliza el sistema para registrar o consultar pedidos, como la propietaria o el personal encargado. |
| **Producto** | Pastel, torta o queque ofrecido por la pastelería. |
| **Fecha de entrega** | Día establecido para entregar el pedido al cliente. |

### 1.4 Referencias

- Propuesta del proyecto integrador: Sistema de gestión de pedidos para la Pastelería Dulce Tentación.
- Instrumento de recolección de información: entrevista, observación directa y revisión documental.
- Norma IEEE 830-1998: Especificación de requisitos de software.

---

## 2. Requerimientos funcionales

Los requerimientos funcionales describen las operaciones que el sistema debe realizar para facilitar la gestión de los pedidos de la pastelería.

| Id | Requerimiento | Prioridad | Origen |
|---|---|---|---|
| RF-01 | El sistema **debe** permitir registrar un pedido indicando el nombre del cliente, número de teléfono, producto solicitado, cantidad y fecha de entrega. | Alta | Objetivo general de la propuesta. |
| RF-02 | El sistema **debe** rechazar el registro de un pedido cuando falte el nombre del cliente, el número de teléfono, el producto, la cantidad o la fecha de entrega. | Alta | Observación del 18/11: se encontró un pedido sin el teléfono del cliente. |
| RF-03 | El sistema **debe** almacenar los pedidos registrados en una base de datos MySQL para conservar la información. | Alta | Objetivo específico 1 y formulación del problema. |
| RF-04 | El sistema **debe** mostrar un listado de los pedidos pendientes ordenados por fecha de entrega. | Alta | Observación del 18/11: se revisaron varias hojas para conocer los pedidos que debían prepararse. |
| RF-05 | El sistema **debe** permitir consultar los pedidos pendientes de una fecha determinada. | Alta | Objetivo específico 3 y observación del 18/11. |
| RF-06 | El sistema **debe** permitir actualizar el estado de un pedido para marcarlo como entregado. | Alta | Objetivo específico 4 y alcance de la propuesta. |
| RF-07 | El sistema **debe** mostrar los datos principales de cada pedido: cliente, teléfono, producto, cantidad y fecha de entrega. | Alta | Instrumento de recolección y proceso actual de registro. |
| RF-08 | El sistema **debe** permitir consultar los productos registrados de la pastelería para seleccionarlos al realizar un pedido. | Media | Punto de partida y alcance de la propuesta. |
| RF-09 | El sistema **debería** permitir buscar un pedido por el nombre del cliente para facilitar su localización. | Baja | Necesidad de mejorar la búsqueda de información identificada en la formulación del problema. |
| RF-10 | El sistema **debe** permitir realizar copias de seguridad de la base de datos para evitar la pérdida de información. | Media | Objetivo general, justificación técnica y alcance de la propuesta. |

---

## 3. Requerimientos no funcionales

Los requerimientos no funcionales describen las condiciones de uso, facilidad de acceso y características técnicas que debe cumplir el sistema.

Cada requerimiento incluye un criterio que permitirá comprobar si se cumple durante las pruebas.

| Id | Requerimiento | Cómo se verifica |
|---|---|---|
| RNF-01 | El registro de un pedido **debe** completarse en un máximo de **60 segundos**, una vez que el operador tenga los datos del cliente y del encargo. | Cronometrar tres registros de pedidos durante las pruebas con el personal encargado. |
| RNF-02 | El formulario de registro **debe** tener como máximo **cinco campos obligatorios**: cliente, teléfono, producto, cantidad y fecha de entrega. | Contar los campos obligatorios del formulario. |
| RNF-03 | El sistema **debe** visualizarse correctamente en una pantalla móvil de **360 px de ancho**, sin desplazamiento horizontal. | Abrir el sistema en el emulador del navegador con un ancho de 360 px. |
| RNF-04 | Los botones y controles principales **deben** tener un tamaño mínimo de **44 × 44 px** para facilitar su uso desde dispositivos táctiles. | Medir los controles mediante las herramientas de inspección del navegador. |
| RNF-05 | El sistema **debe** conservar los pedidos registrados después de cerrar y volver a abrir el navegador, utilizando la base de datos MySQL. | Registrar un pedido, cerrar el navegador, volver a ingresar y comprobar que el pedido continúa almacenado. |
| RNF-06 | El sistema **debe** permitir su utilización desde un navegador web actual en computadoras y teléfonos celulares. | Realizar pruebas de acceso desde una computadora y un teléfono celular. |
| RNF-07 | El sistema **debe** mostrar los resultados de una consulta de pedidos en un máximo de **3 segundos**, con una base de datos de prueba de hasta 500 pedidos y conexión local. | Ejecutar cinco consultas y medir el tiempo de respuesta. |
| RNF-08 | El sistema **debe** validar los campos obligatorios antes de guardar un pedido, mostrando un mensaje cuando falte información. | Intentar guardar pedidos con uno o más campos obligatorios vacíos. |

---

## 4. Requerimientos omitidos de la norma

La norma IEEE 830-1998 contempla diferentes aspectos de especificación que no son necesarios para el alcance actual del proyecto. Por ello, se omiten explícitamente los siguientes:

- **Interfaces de hardware:** el sistema no requiere comunicación directa con impresoras, lectores de códigos de barras u otros dispositivos especializados.
- **Interfaces con otros sistemas:** durante esta etapa no se contempla la integración con sistemas externos de pagos, facturación o mensajería.
- **Requisitos de tiempo real:** el sistema no requiere procesamiento en tiempo real ni tiene restricciones especiales de latencia más allá de los tiempos de respuesta establecidos.
- **Gestión de varias sucursales:** el sistema está destinado únicamente a la Pastelería Dulce Tentación ubicada en Colquencha.
- **Portabilidad entre sistemas operativos:** al tratarse de una aplicación web, se accederá mediante navegadores compatibles, sin necesidad de instalar una aplicación específica para cada sistema operativo.

Estas características podrán considerarse en futuras versiones si las necesidades de la pastelería aumentan.

---

## 5. Consideraciones para la verificación

Los requerimientos definidos serán utilizados durante las pruebas del sistema para comprobar que las funcionalidades desarrolladas respondan a las necesidades identificadas.

Se realizarán las siguientes verificaciones:

| Prueba | Aspecto que se comprobará |
|---|---|
| Registro de pedidos | Que los pedidos se guarden correctamente con todos sus datos. |
| Validación de campos | Que no se permita registrar pedidos con información obligatoria incompleta. |
| Consulta de pedidos | Que se visualicen los pedidos pendientes y se puedan filtrar por fecha de entrega. |
| Actualización del estado | Que un pedido pueda marcarse como entregado. |
| Conservación de información | Que los pedidos permanezcan almacenados después de cerrar el navegador. |
| Adaptación móvil | Que el sistema pueda utilizarse correctamente desde un teléfono celular. |
| Respaldo de información | Que se pueda generar una copia de seguridad de la base de datos. |

---

## 6. Conclusión

La presente especificación establece los requerimientos funcionales y no funcionales del sistema de gestión de pedidos para la Pastelería Dulce Tentación.

Estos requerimientos se definieron considerando la información obtenida mediante la entrevista, la observación directa y la revisión del cuaderno de pedidos.

Su cumplimiento permitirá desarrollar un sistema que facilite el registro de los encargos, evite la omisión de datos importantes, reduzca el tiempo de búsqueda de pedidos y mejore el seguimiento de las fechas de entrega.

Además, esta especificación servirá como referencia para la etapa de construcción y para la elaboración de la matriz de casos de prueba del proyecto integrador.