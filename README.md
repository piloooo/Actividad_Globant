# Actividad_Globant - Proyecto Appetito
- Propósito del Sistema:
Appetito es una Webapp cuyo objetivo es modernizar y simplificar el proceso de compra y reserva de alimentos dentro de instituciones educativas.

La aplicación busca resolver dos problemas principales:

*Control y Logística: Permite a los padres realizar la compra y reserva de productos para sus hijos con anticipación, facilitando un control sobre el tipo de alimentos que consumen.

*Reducción de Efectivo: Elimina la necesidad de que los estudiantes lleven dinero en efectivo a la institución, ya que todas las transacciones se gestionan a través de un sistema de saldo cargado por los padres.

En resumen, Appetito actúa como un intermediario digital que optimiza la operación del kiosco y ofrece tranquilidad y control a la comunidad educativa.

- Arquitectura del Sistema y Documentación
Para documentar la arquitectura de Appetito, hemos desarrollado los siguientes diagramas. Se utilizó la herramienta Lucidchart para su creación.

1. Diagrama de Bloques (Arquitectura General)
Este diagrama representa la estructura de alto nivel y la interconexión de los componentes tecnológicos esenciales del sistema:

*Interfaz (Frontend): La capa con la que interactúan los padres.

*Servidor de Webapp (Backend): Contiene la lógica de negocio, procesa las solicitudes y coordina la comunicación con la base de datos.

*Base de Datos: El almacenamiento central de todos los datos críticos (usuarios, saldos, pedidos, menú, etc.).

*Interfaz de Administración (Kiosquero): Un módulo específico para que el personal del kiosco pueda gestionar pedidos pendientes y stock.

2. Diagrama de Flujo (Proceso de Compra del Cliente)
Este diagrama de secuencia ilustra el camino que sigue un usuario (padre) al interactuar con la aplicación para realizar una compra:

*Muestra el flujo de ingreso, incluyendo la validación inicial de ¿Tiene cuenta? (Registro o Ingreso).

*Detalla los pasos funcionales: Elegir un producto y Agregar al carrito.

*Resalta un punto de decisión crítico: la verificación de ¿Tienes saldo suficiente?.

*El flujo concluye con la Confirmar compra, asegurando que solo se procesen pedidos validados.

3. Diagrama de Casos de Uso (UML)
Este diagrama describe las funciones del sistema desde la perspectiva de sus dos actores principales, el Cliente (Padre) y el Kiosco (Kiosquero):

*Cliente (Padre): Realiza funciones como Registrarse, Agregar saldo y Hacer pedido.

*Kiosco (Kiosquero): Sus funciones se centran en la gestión operativa: ver Pedidos del día y Cargar menú.

*Las relaciones de inclusión (líneas punteadas) como Verificar saldo y Verificar DNI muestran que ciertas acciones complejas dependen de procesos de validación internos.

4. Diagrama Entidad-Relación (ER)
*Este diagrama representa la estructura lógica de la base de datos, vital para garantizar la Coherencia Técnica del proyecto:

*Muestra las principales entidades que almacenan datos del sistema: Padre, Alumno, Kiosco, Producto, Pedido y Detalle.

*Define las relaciones entre ellas. Por ejemplo, la entidad Pedido está directamente relacionada con Padre y con Alumno.

*La tabla Detalle es crucial, ya que vincula el Pedido con los Productos específicos, permitiendo conocer el subtotal y la cantidad de cada ítem.

Herramientas Utilizadas
Todos los diagramas fueron creados utilizando la herramienta Lucidchart
