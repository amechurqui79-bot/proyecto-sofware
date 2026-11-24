# Sistema de gestión de pedidos para la Pastelería Dulce Tentación

**Propuesta de Proyecto Integrador**

Programa Académico Desconcentrado  
**Técnico Superior en Informática – UMSA**  
Sede Colquencha

**Autora:** Amalia Patty Churqui  
**Fecha:** Noviembre de 2026

---

## 1. Tipo de proyecto

**Proyecto integrador.**

El presente proyecto consiste en desarrollar un sistema de software que permita solucionar una necesidad concreta de la Pastelería Dulce Tentación. Para ello, se construirá una aplicación web que facilite el registro, almacenamiento y consulta de los pedidos realizados por los clientes.

El proyecto no se limita a presentar una investigación teórica, sino que busca desarrollar una solución funcional que responda a las necesidades del negocio. También contará con documentación técnica, pruebas de funcionamiento y una propuesta para su puesta en producción.

## 2. Punto de partida

El presente proyecto continúa con el trabajo realizado en el módulo de Programación Web, donde se desarrolló la página web de la Pastelería Dulce Tentación. Esta página permite mostrar los productos que ofrece el negocio, como tortas, pasteles y queques, además de presentar información sobre la pastelería.

En la primera etapa se trabajó en el diseño de la página, utilizando HTML, CSS y JavaScript. También se incorporó información de los productos mediante un archivo JSON para facilitar su presentación.

Sin embargo, todavía es necesario mejorar algunas funciones, principalmente el registro y control de los pedidos que realizan los clientes. Actualmente, estos encargos se anotan en un cuaderno físico, lo que dificulta su organización y consulta.

Por esta razón, en este módulo se propone completar el proyecto mediante el desarrollo de un sistema web que permita registrar los pedidos, almacenar la información en una base de datos y consultar los encargos según su fecha de entrega.

| Ya existe                                          | Se desarrollará en este módulo                               |
|____________________________________________________|______________________________________________________________|
| Página web de la Pastelería Dulce Tentación.       | Propuesta que justifica el desarrollo del sistema.           |
| Diseño de la página con HTML, CSS y JavaScript.    | Base de datos para almacenar clientes, productos y pedidos.  |
| Información de los productos en un archivo JSON.   | Registro de nuevos pedidos desde la página web.              |
| Presentación de los productos y datos del negocio. | Consulta de pedidos pendientes por fecha de entrega.         |
| Página web publicada.                              | Pruebas, respaldo de información y puesta en producción.     |
## 3. El cliente

La Pastelería Dulce Tentación es un negocio ubicado en la Av. La Paz 45, localidad de Colquencha, departamento de La Paz. Se dedica a la elaboración y venta de pasteles, tortas y queques para el público en general. También recibe pedidos por encargo para diferentes ocasiones.

El negocio cuenta con una forma de trabajo tradicional para registrar los encargos de sus clientes. Cuando una persona realiza un pedido, se anotan en un cuaderno los datos del cliente, el producto que solicita, la cantidad y la fecha en la que debe entregarse.

Aunque este método permite llevar un registro de los pedidos, presenta algunas dificultades al momento de buscar información, revisar qué encargos deben prepararse y recordar las fechas de entrega. Además, al estar toda la información en un cuaderno físico, existe el riesgo de que los datos se pierdan o se deterioren.

Por esta razón, se plantea desarrollar un sistema web que ayude a la Pastelería Dulce Tentación a organizar mejor sus pedidos, consultar los encargos pendientes y guardar la información de manera digital.

Fuente de información: entrevista realizada a la propietaria de la Pastelería Dulce Tentación el 14 de noviembre de 2026.
## 4. Formulación del problema

La Pastelería Dulce Tentación registra actualmente los pedidos por encargo en un cuaderno físico ubicado en el mostrador. En este cuaderno se anotan los datos del cliente, el producto solicitado, la cantidad y la fecha en la que debe entregarse.

Sin embargo, el registro manual presenta algunas dificultades para la organización del negocio.

**Pérdida o falta de seguimiento de pedidos.** Al registrar los encargos manualmente, existe la posibilidad de que algunos pedidos no sean revisados a tiempo o que se pase por alto su fecha de entrega. Esto puede ocasionar retrasos, confusiones y reclamos por parte de los clientes.

**Dificultad para consultar los pedidos.** Cuando se necesita conocer los encargos que deben prepararse en una fecha determinada, es necesario revisar las anotaciones del cuaderno. Como los pedidos se registran según el orden de llegada, su búsqueda puede tomar tiempo y dificultar la organización de las actividades diarias.

**Ausencia de respaldo de la información.** El cuaderno físico es el principal medio de almacenamiento de los pedidos. Si se pierde, se deteriora o se daña, la información registrada puede desaparecer y sería difícil recuperar los datos de los encargos anteriores.

Estas dificultades muestran la necesidad de contar con un sistema que permita registrar los pedidos de manera organizada, consultar las fechas de entrega y conservar la información mediante una base de datos.

### 4.1. Árbol de problemas

**Efectos**

- Retrasos en la preparación y entrega de algunos pedidos.
- Pérdida de información de los encargos registrados.
- Tiempo adicional para buscar y revisar los pedidos.
- Posibles reclamos y molestias de los clientes.

**Problema central**

El registro manual de los pedidos por encargo de la Pastelería Dulce Tentación dificulta la organización, consulta y seguimiento de las fechas de entrega, lo que puede ocasionar confusiones y pedidos no atendidos a tiempo.

**Causas**

- Los pedidos se registran en un cuaderno físico.
- La información se organiza según el orden de llegada y no por fecha de entrega.
- No existe una base de datos para almacenar los pedidos.
- No se cuenta con un respaldo digital de la información.
- La consulta de los encargos depende de la revisión manual del cuaderno.

### 4.2. Problema central

> El registro manual de los pedidos por encargo de la Pastelería Dulce Tentación dificulta la consulta y el seguimiento de las fechas de entrega, lo que puede ocasionar confusiones, retrasos y pérdida de información.

## 5. Objetivos

### 5.1. Objetivo general

Desarrollar un sistema web de gestión de pedidos para la Pastelería Dulce Tentación, que permita registrar los encargos de los clientes, consultar los pedidos pendientes según su fecha de entrega y almacenar la información en una base de datos para mejorar su organización y seguimiento.

### 5.2. Objetivos específicos

1. Diseñar una base de datos relacional que permita almacenar y organizar la información de los clientes, productos y pedidos de la pastelería.

2. Implementar un módulo de registro de pedidos que permita ingresar los datos del cliente, el producto solicitado, la cantidad y la fecha de entrega.

3. Desarrollar una opción de consulta que permita visualizar los pedidos pendientes y filtrarlos según la fecha de entrega.

4. Verificar el funcionamiento del sistema mediante casos de prueba que permitan comprobar el registro, almacenamiento, consulta y actualización del estado de los pedidos.

## 6. Justificación

### 6.1. Justificación práctica

El proyecto se realiza debido a las dificultades que presenta la Pastelería Dulce Tentación al registrar sus pedidos de forma manual en un cuaderno. Este procedimiento puede ocasionar confusiones al momento de buscar los encargos y recordar las fechas en las que deben entregarse.

Con el desarrollo del sistema web, la propietaria podrá registrar los pedidos y consultar los encargos pendientes de manera más rápida y ordenada. También podrá identificar qué productos fueron solicitados, en qué cantidad y para qué fecha deben estar preparados.

De esta manera, se busca mejorar la organización de los pedidos y reducir los errores que pueden presentarse durante la atención a los clientes.

### 6.2. Justificación técnica

Se propone desarrollar un sistema web porque permite acceder a la información desde diferentes dispositivos, como computadoras, laptops y teléfonos celulares, siempre que se cuente con un navegador y conexión a internet cuando el sistema esté publicado.

Para su desarrollo se utilizarán tecnologías como HTML, CSS y JavaScript para la interfaz, PHP para el procesamiento de la información y MySQL para el almacenamiento de los datos.

Además, el sistema permitirá guardar la información en una base de datos, facilitando su consulta y la realización de copias de respaldo cuando sea necesario.

### 6.3. Justificación social

El sistema beneficiará principalmente a la propietaria y al personal encargado de atender los pedidos en la Pastelería Dulce Tentación, porque facilitará el trabajo diario y permitirá tener un mejor control de los encargos.

También beneficiará a los clientes, ya que una mejor organización ayudará a reducir las confusiones relacionadas con los productos solicitados y sus fechas de entrega.

De esta manera, se busca brindar una atención más ordenada y mejorar la comunicación entre la pastelería y sus clientes.

## 7. Factibilidad

### 7.1. Factibilidad técnica

El desarrollo del sistema es técnicamente posible porque se utilizarán herramientas y tecnologías conocidas durante la formación académica.

Para la programación y las pruebas locales se utilizará Visual Studio Code y XAMPP, que permitirá trabajar con PHP y MySQL. Posteriormente, el sistema podrá publicarse en un servicio de alojamiento web que admita estas tecnologías.

El proyecto aprovechará la página web desarrollada anteriormente en el módulo de Programación Web, por lo que no será necesario comenzar desde cero.

### 7.2. Factibilidad operativa

El sistema estará destinado principalmente a la propietaria y al personal encargado de registrar y revisar los pedidos.

Su funcionamiento será sencillo, ya que contará con opciones para registrar nuevos pedidos, consultar los encargos pendientes y actualizar su estado cuando hayan sido entregados.

Además, podrá utilizarse desde un teléfono celular o una computadora mediante un navegador web, evitando la instalación de programas adicionales.

**Riesgo identificado:** para que el sistema funcione correctamente, los pedidos deberán registrarse en el momento en que sean solicitados. Si se continúa anotando primero en el cuaderno y después se pasan los datos al sistema, podrían mantenerse los mismos problemas de organización.

Para reducir este riesgo, se propone que el sistema esté disponible desde el dispositivo utilizado en el mostrador de la pastelería.

### 7.3. Factibilidad económica

El desarrollo del sistema se realizará como parte del proyecto académico, por lo que no se considera un costo de programación para la pastelería.

Sin embargo, para mantener el sistema publicado se deberán considerar los posibles gastos de alojamiento web y dominio.

Los siguientes montos son estimaciones referenciales que deberán verificarse antes de contratar el servicio:

| Concepto | Costo anual estimado (Bs) |
|---|---:|
| Hosting compartido con PHP y MySQL | 350 |
| Dominio web | 250 |
| **Total estimado** | **600** |

La propietaria deberá evaluar si puede cubrir estos gastos para mantener el sistema disponible en internet. También se podrá considerar inicialmente un entorno local para realizar pruebas sin asumir costos de alojamiento.

## 8. Alcances y límites

### 8.1. Alcances

El sistema web de gestión de pedidos para la Pastelería Dulce Tentación tendrá las siguientes funcionalidades:

- **Registro de pedidos:** permitirá ingresar el nombre del cliente, el producto solicitado, la cantidad y la fecha de entrega.
- **Consulta de pedidos:** permitirá visualizar los pedidos registrados y buscar los pendientes según la fecha de entrega.
- **Actualización del estado:** permitirá marcar los pedidos como entregados una vez que hayan sido preparados y entregados al cliente.
- **Listado de productos:** permitirá consultar los productos disponibles de la pastelería, como pasteles y queques.
- **Almacenamiento de información:** permitirá guardar los datos de clientes, productos y pedidos en una base de datos MySQL.
- **Respaldo de información:** permitirá realizar copias de seguridad de la base de datos para evitar la pérdida de los registros.

### 8.2. Límites

El sistema no incluirá las siguientes funcionalidades durante esta etapa del proyecto:

- **Cobros y facturación:** no se desarrollará un módulo de facturación ni de pagos electrónicos, debido a que el objetivo principal es mejorar el registro y seguimiento de los pedidos.
- **Gestión de inventario e insumos:** no se incluirá el control de materias primas, como harina, azúcar, huevos y otros ingredientes, porque el proyecto se concentra en la administración de los encargos.
- **Notificaciones automáticas:** no se implementará el envío automático de mensajes a los clientes mediante WhatsApp o SMS, ya que requiere servicios e integraciones adicionales.
- **Administración de varias sucursales:** el sistema estará destinado al funcionamiento de un solo establecimiento, correspondiente a la Pastelería Dulce Tentación en Colquencha.

Estas funcionalidades podrán considerarse como mejoras para futuras versiones del sistema.

## 9. Cronograma de actividades

### 9.1. Descomposición del trabajo

**1. Propuesta**

- 1.1. Formulación del problema.
- 1.2. Elaboración de objetivos y justificación.
- 1.3. Análisis de factibilidad, alcances y límites.
- 1.4. Elaboración del cronograma.

**2. Análisis**

- 2.1. Elaboración del instrumento de recolección de información y realización de la entrevista.
- 2.2. Desarrollo del marco teórico.
- 2.3. Identificación de requerimientos funcionales y no funcionales.
- 2.4. Elaboración de historias de usuario.

**3. Construcción**

- 3.1. Diseño y creación de la base de datos.
- 3.2. Desarrollo de las funcionalidades de registro y consulta de pedidos.
- 3.3. Conexión del frontend con el backend.

**4. Verificación y cierre**

- 4.1. Elaboración y ejecución de la matriz de casos de prueba.
- 4.2. Realización del respaldo de la información y preparación de la puesta en producción.
- 4.3. Elaboración del documento final y preparación de la defensa del proyecto.

### 9.2. Cronograma

| Semana | Fechas | Actividades | Entregable |
|---|---|---|---|
| 1 | 23 al 29 de noviembre de 2026 | Formulación del problema, objetivos, justificación, factibilidad y alcances. | Propuesta del proyecto completa. |
| 2 | 30 de noviembre al 6 de diciembre de 2026 | Entrevista, marco teórico, requerimientos e historias de usuario. | Documento de análisis del sistema. |
| 3 | 7 al 13 de diciembre de 2026 | Diseño de la base de datos, desarrollo del backend y conexión con el frontend. | Sistema conectado a la base de datos. |
| 4 | 14 al 20 de diciembre de 2026 | Pruebas, respaldo, documentación final y preparación de la defensa. | Sistema verificado y documento final. |

## 10. Resumen

La Pastelería Dulce Tentación, ubicada en Colquencha, se dedica a la elaboración y venta de pasteles y queques. Actualmente, los pedidos por encargo se registran manualmente en un cuaderno, donde se anotan los datos del cliente, el producto solicitado, la cantidad y la fecha de entrega. Esta forma de trabajo puede ocasionar dificultades al momento de consultar los pedidos pendientes, organizar las fechas de entrega y conservar la información.

Ante esta situación, el presente proyecto propone desarrollar un sistema web de gestión de pedidos que permita registrar los encargos de los clientes, consultar los pedidos pendientes por fecha de entrega y actualizar su estado cuando hayan sido entregados.

El sistema se desarrollará utilizando HTML, CSS y JavaScript para la interfaz, PHP para el procesamiento de los datos y MySQL para almacenar la información. Además, se aprovechará la página web elaborada anteriormente en el módulo de Programación Web.

Finalmente, se realizarán pruebas para comprobar que las funcionalidades del sistema trabajen correctamente y se establecerá un procedimiento de respaldo de la base de datos. Con este proyecto se busca mejorar la organización de los pedidos y facilitar el trabajo diario de la Pastelería Dulce Tentación.

## 11. Introducción

El presente documento describe el desarrollo de un sistema web de gestión de pedidos para la Pastelería Dulce Tentación, como parte del Proyecto Integrador del Programa Académico Desconcentrado Técnico Superior en Informática de la Universidad Mayor de San Andrés (UMSA), Sede Colquencha.

El proyecto surge a partir de la necesidad de mejorar la manera en que se registran y organizan los pedidos por encargo de la pastelería. Actualmente, estos datos se anotan en un cuaderno físico, lo que puede dificultar su búsqueda, el seguimiento de las fechas de entrega y la conservación de la información.

Como una primera parte del trabajo, en el módulo de Programación Web se desarrolló una página web para mostrar los productos y la información del negocio. Sin embargo, esta versión inicial no cuenta con una base de datos que permita almacenar y administrar los pedidos realizados por los clientes. Por esta razón, en el presente módulo se propone completar el sistema mediante la incorporación de PHP y MySQL.

El sistema permitirá registrar nuevos pedidos, consultar los encargos pendientes según su fecha de entrega y actualizar su estado. De esta manera, se pretende facilitar la organización de las actividades de la pastelería y reducir las dificultades que presenta el registro manual.

El documento está organizado en diferentes partes. En primer lugar, se presenta la propuesta del proyecto, donde se explica el problema identificado, los objetivos, la justificación, la factibilidad y los alcances. Posteriormente, se desarrolla el análisis del sistema mediante la recopilación de información, el marco teórico y los requerimientos. Después, se describe el proceso de construcción, incluyendo el diseño de la base de datos y la implementación de las funcionalidades. Finalmente, se presentan las pruebas realizadas, los aspectos relacionados con la puesta en producción, las conclusiones y las recomendaciones.

---
