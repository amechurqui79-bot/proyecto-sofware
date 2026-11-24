# Marco teórico

## Sistema de gestión de pedidos para la Pastelería Dulce Tentación

---

## Introducción

El registro de pedidos por encargo es una actividad importante para el funcionamiento de una pastelería. Existen diferentes alternativas para organizar esta información, desde el uso de cuadernos y planillas de cálculo hasta aplicaciones comerciales y sistemas desarrollados a medida.

Este apartado revisa cuatro alternativas para la gestión de pedidos y analiza por qué ninguna se ajusta completamente a las condiciones de la Pastelería Dulce Tentación. A partir de esta comparación se fundamenta la propuesta de desarrollar un sistema web que permita registrar pedidos y consultarlos por fecha de entrega, de acuerdo con las necesidades del establecimiento.

## Estado del arte

### Alternativas existentes

| Solución | Costo | Sin internet | Desde celular | Consulta por fecha |
|---|---|---|---|---|
| **Cuaderno de papel** *(actual)* | Bs 0 | sí | no aplica | no, búsqueda manual |
| **Planilla de cálculo compartida** | Bs 0 | no, si es en línea | posible, pero poco práctica | sí, con filtros |
| **Software de gestión comercial** *(genérico)* | según proveedor | según el producto | generalmente sí | sí, entre varias funciones |
| **Sistema a medida** | depende del desarrollo | depende de su implementación | sí, si es adaptable | sí |
| **Solución propuesta** | Bs 600/año | no *(requiere conexión)* | sí | sí |

### Análisis

**El cuaderno** es el método utilizado actualmente por la Pastelería Dulce Tentación. No tiene costo y permite registrar pedidos sin necesidad de electricidad ni conexión a internet. Sin embargo, presenta dificultades para encontrar rápidamente los encargos y consultar cuáles deben entregarse en una fecha determinada. También existe el riesgo de perder o deteriorar la información. Se mantendrá como respaldo de contingencia cuando el sistema no esté disponible.

**La planilla compartida** permite organizar los datos de los clientes, productos, cantidades y fechas de entrega. También facilita la búsqueda mediante filtros. Su principal limitación es que, cuando se utiliza en línea, necesita conexión a internet. Además, puede resultar poco práctica para registrar pedidos rápidamente desde un celular durante la atención a los clientes.

**El software de gestión comercial** ofrece funciones para administrar ventas, inventario, clientes y otros procesos de un negocio. Aunque puede resolver el problema del registro de pedidos, incluye herramientas que no son necesarias para las actividades actuales de la pastelería. Por ello, su costo y complejidad pueden resultar innecesarios para un establecimiento pequeño.

**El sistema a medida** permite desarrollar funciones de acuerdo con las necesidades específicas del negocio. Puede adaptarse al registro de clientes, productos, cantidades y fechas de entrega. Sin embargo, requiere tiempo de desarrollo, mantenimiento y recursos económicos para su implementación y funcionamiento.

### Conclusión del estado del arte

Ninguna de las alternativas analizadas responde completamente a las necesidades de la Pastelería Dulce Tentación. El cuaderno permite trabajar sin internet, pero dificulta la búsqueda de pedidos. Las planillas facilitan las consultas, aunque pueden resultar poco prácticas desde un celular. Por otro lado, los programas comerciales pueden incluir funciones y costos que no se justifican para las necesidades del establecimiento.

Por esta razón, se propone desarrollar un sistema web que permita registrar los pedidos, almacenar los datos de los clientes y productos, consultar los encargos pendientes por fecha de entrega y actualizar su estado cuando sean entregados.

La solución propuesta tiene una limitación importante: necesita conexión a internet para funcionar en línea. Esta desventaja se tendrá en cuenta manteniendo el cuaderno como respaldo de contingencia cuando exista algún problema de conexión. Además, se realizarán exportaciones periódicas de la base de datos para conservar copias de seguridad y evitar la pérdida de información.

De esta manera, el sistema se adaptará a las condiciones de la pastelería y permitirá mejorar la organización y el control de los pedidos sin incorporar funciones innecesarias.

## Metodología de desarrollo

Se adopta un **enfoque incremental**, porque permite desarrollar el sistema por etapas y comprobar el funcionamiento de cada parte antes de continuar con la siguiente. Esta metodología resulta adecuada para el proyecto, considerando que el tiempo disponible para el desarrollo es de aproximadamente cuatro semanas.

No se aplicará Scrum en su forma completa, porque el proyecto no cuenta con todos los roles y actividades que requiere esa metodología. En su lugar, se organizará el trabajo mediante entregas progresivas, revisiones y pruebas de las funcionalidades desarrolladas.

Las etapas de trabajo serán las siguientes:

| Etapa | Actividad |
|---|---|
| Primera semana | Identificación de necesidades y definición de requerimientos del sistema. |
| Segunda semana | Diseño de la base de datos y organización de la estructura del sistema. |
| Tercera semana | Desarrollo de las funciones de registro y consulta de pedidos y administración de productos. |
| Cuarta semana | Pruebas, corrección de errores y verificación del funcionamiento del sistema. |

### Herramientas

| Herramienta | Uso | Por qué |
|---|---|---|
| HTML, CSS y JavaScript | interfaz del sistema | permiten construir y adaptar la página web que ya se inició en el módulo anterior. |
| PHP 8 | procesamiento del servidor | permite procesar los datos y realizar las operaciones del sistema. |
| MySQL | almacenamiento de información | permite guardar y organizar los datos de clientes, productos y pedidos. |
| XAMPP | entorno de desarrollo local | permite probar el sistema en una computadora antes de publicarlo. |
| Git y GitHub | control de versiones | permiten conservar el historial de cambios y recuperar versiones anteriores del código. |
| Matriz de casos de prueba | verificación | permite comprobar que el registro, la consulta y la actualización de pedidos funcionen correctamente. |

---

## Referencias bibliográficas

Contreras Núñez, R. A., & Moraga Mancilla, A. E. (2012). *Sistema de gestión de pedidos y seguimiento de clientes* [Tesis de Ingeniería en Computación e Informática, Universidad Andrés Bello]. Repositorio Institucional de la Universidad Andrés Bello. http://repositorio.unab.cl/xmlui/handle/ria/11177

Elmasri, R., & Navathe, S. B. (2016). *Fundamentals of database systems* (7th ed.). Pearson.

Flores Ricaldez, M. M. (2021). *Implementación de la aplicación móvil de pedido para la panadería* [Tesis de licenciatura, Universidad Autónoma Gabriel René Moreno]. Catálogo de Tesis del Sistema Integrado de Bibliotecas Digitales de la UAGRM. https://bibliotecas.uagrm.edu.bo/opac_web/catalogo_de_tesis/?ind=I&page=13&url=opac_web%2Fcatalogo_de_tesis%2F&view=details

Pressman, R. S., & Maxim, B. R. (2020). *Software engineering: A practitioner's approach* (9th ed.). McGraw-Hill.

Quijije Anchundia, P. del R., & Lucas López, A. R. (2018). *Análisis, desarrollo e implementación de una aplicación basado en tecnología web y móvil para la gestión de ventas y control de pedidos en línea en Pastelería Dayana del cantón Montecristi* [Trabajo de titulación, Universidad Laica Eloy Alfaro de Manabí]. Repositorio Institucional ULEAM. https://repositorio.uleam.edu.ec/bitstream/123456789/1134/1/ULEAM-INFOR-0026.pdf

Romero De La A., N. E. (2026). *Desarrollo de una aplicación web para la gestión y control de pedidos de la panadería y pastelería Rey Pan* [Trabajo de titulación, Universidad Estatal Península de Santa Elena]. Repositorio Institucional UPSE. https://repositorio.upse.edu.ec/handle/46000/16027

### Fuentes no bibliográficas

La información sobre el funcionamiento actual de la Pastelería Dulce Tentación proviene de las siguientes fuentes:

- Entrevista semiestructurada a la propietaria de la pastelería.
- Observación directa del proceso de recepción y registro de pedidos, realizada el 18 de noviembre de 2026.
- Revisión del cuaderno utilizado para registrar los pedidos.
- Revisión de los registros de pedidos y de las dificultades presentadas durante su organización.

Estas fuentes permiten conocer el procedimiento actual, identificar los problemas del registro manual y establecer las necesidades que deberá atender el sistema web.

## Nota sobre integridad académica

Este documento utiliza antecedentes de proyectos académicos y libros relacionados con el desarrollo de software y la administración de bases de datos. Las ideas obtenidas de otros autores se identifican mediante sus respectivas citas y referencias bibliográficas.

La descripción de los problemas de la Pastelería Dulce Tentación y las decisiones tomadas para desarrollar el sistema se fundamentan en la información recopilada mediante entrevistas, observación directa y revisión documental.