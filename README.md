# YuVa's adventure

## Descripción

YuVa's adventure es un negocio especializado en juegos de mesa y juegos de rol, ubicado a las afueras de Tobarra (Albacete). Su propósito es ofrecer a los jugadores nuevas formas de disfrutar de sus aficiones y de vivir experiencias únicas, tanto a través de sus productos como de sus servicios.

Hasta ahora, la actividad del negocio se ha limitado a la venta directa en tienda. Con el fin de llegar a más jugadores y de facilitar el acceso a su oferta, la empresa ha decidido comenzar a vender y promocionar sus productos y servicios de manera online, y para ello necesita una aplicación web que centralice toda su actividad:

- **Venta de productos:** juegos de mesa, de rol y complementos.
- **Eventos de rol:** organización de partidas de rol clásico y en vivo. Dirigidas por másteres experimentados.
- **Alquiler de salas:** reserva de salas y espacios de nuestras instalaciones para jugar con tus amigos.
- **Comunidad de jugadores:** grupos privados donde los usuarios puedan compartir fotos y comentarios de sus partidas.

## Objetivo

### Objetivo general

Desarrollar una aplicación web que cubra las necesidades de negocio de YuVa's adventure, permitiéndole vender sus productos, gestionar sus eventos, reservas de salas y fomentar una comunidad de jugadores en torno a su actividad.

### Objetivos específicos

- Ofrecer a los clientes una tienda online completa, desde la consulta del catálogo hasta el pago y el seguimiento de sus pedidos.
- Permitir la inscripción a eventos de rol y la reserva de salas de forma sencilla, controlando las plazas y la disponibilidad.
- Facilitar la creación de grupos privados de clientes donde compartir fotos y comentarios, con mecanismos de reporte y moderación.
- Proporcionar al personal herramientas para gestionar el catálogo, el stock, los pedidos, los eventos, las salas y la moderación de contenidos.
- Dar al administrador el control total del sistema, incluyendo cuentas, categorías, promociones y estadísticas de actividad.
- Automatizar tareas repetitivas, como el envío de notificaciones por email y la actualización de estados y stock, para reducir la carga de trabajo manual.

## Roles

| Nombre | Descripción |
| :---: | :---: |
| Invitado | Usuario que no haya iniciado sesión |
| Cliente | Usuario registrado en la aplicación |
| Trabajador | Usuario con acceso a la gestión del inventario y moderación de mensajes |
| Administrador | Usuario con control total del sistema |
| Sistema | Procesos automáticos de la aplicación |

## Requisitos funcionales

| ID | Rol | Requisito | Descripción | Prioridad |
| :---: | :---: | :---: | :---: | :---: |
| RF-01 | Invitado, Cliente, Trabajador, Administrador | Consultar catálogo | Podrá visualizar los productos ofertados, con su precio promocional si lo tienen | Alta |
| RF-02 | Invitado, Cliente, Trabajador, Administrador | Buscar productos | Podrá buscar productos en el buscador mediante palabras clave | Baja |
| RF-03 | Invitado, Cliente, Trabajador, Administrador | Filtrar productos | Podrá filtrar los productos por categorías preestablecidas | Alta |
| RF-04 | Invitado, Cliente, Trabajador, Administrador | Visualizar un producto | Podrá visualizar la información de un producto seleccionado, con su precio promocional si lo tiene | Alta |
| RF-05 | Trabajador, Administrador | Gestionar productos | Podrá visualizar, añadir, modificar o eliminar los productos del catálogo | Alta |
| RF-06 | Administrador | Gestionar categorías | Podrá añadir, modificar o eliminar categorías de producto | Alta |
| RF-07 | Administrador | Gestionar palabras clave del buscador | Podrá añadir, modificar o eliminar las palabras clave asociadas a los productos para el buscador | Baja |
| RF-08 | Trabajador, Administrador | Gestionar stock | Podrá consultar y modificar las unidades disponibles de cada producto | Alta |
| RF-09 | Invitado | Registrarse | Podrá crear una cuenta de cliente | Alta |
| RF-10 | Sistema | Verificar email | Enviará un email de verificación al registrarse y no permitirá realizar pedidos, reservas ni inscripciones hasta que la cuenta esté verificada | Media |
| RF-11 | Invitado | Iniciar sesión | Podrá acceder al sistema mediante sus credenciales | Alta |
| RF-12 | Sistema | Bloquear cuenta por intentos fallidos | Bloqueará temporalmente el acceso tras varios inicios de sesión fallidos consecutivos | Baja |
| RF-13 | Cliente, Trabajador, Administrador | Cerrar sesión | Podrá cerrar su sesión | Alta |
| RF-14 | Cliente, Trabajador, Administrador | Recuperar contraseña | Podrá solicitar una nueva contraseña por email | Media |
| RF-15 | Sistema | Enviar recuperación de contraseña | Enviará por email el enlace o la nueva contraseña cuando se solicite recuperarla | Media |
| RF-16 | Cliente | Gestionar perfil | Podrá modificar sus datos personales y de envío | Alta |
| RF-17 | Trabajador, Administrador | Modificar sus credenciales | Podrá modificar su contraseña y el email asociado | Media |
| RF-18 | Administrador | Crear cuentas de Trabajador y Administrador | Podrá crear las cuentas especiales de Trabajador y Administrador | Alta |
| RF-19 | Administrador | Gestionar cuentas | Podrá modificar y eliminar cualquier cuenta | Alta |
| RF-20 | Cliente | Gestionar carrito | Podrá visualizar, añadir o eliminar productos de su carrito | Alta |
| RF-21 | Cliente | Realizar pedido | Podrá confirmar los productos de su carrito, la dirección de envío y el método de pago | Alta |
| RF-22 | Sistema | Verificar stock | Comprobará la disponibilidad de los productos al confirmar un pedido y lo rechazará si no hay unidades suficientes | Alta |
| RF-23 | Cliente | Pagar pedido | Podrá acceder a la pasarela de pago seleccionada para pagar su pedido | Alta |
| RF-24 | Sistema | Actualizar estado tras el pago | Marcará el pedido como Pagado cuando la pasarela confirme el pago | Alta |
| RF-25 | Sistema | Gestionar pago rechazado | Si la pasarela rechaza o no completa el pago, mantendrá el pedido pendiente de pago e informará al cliente | Media |
| RF-26 | Sistema | Actualizar stock | Descontará del inventario las unidades de un pedido cuando se confirme su pago y las repondrá si el pedido se cancela | Alta |
| RF-27 | Sistema | Enviar detalles del pedido | Enviará por email al cliente los detalles de su pedido al registrarlo | Media |
| RF-28 | Cliente | Consultar historial de pedidos | Podrá visualizar sus pedidos con su estado, productos y coste | Media |
| RF-29 | Cliente | Cancelar pedido | Podrá cancelar un pedido siempre que no haya sido enviado | Media |
| RF-30 | Sistema | Reembolsar pedido cancelado | Solicitará a la pasarela el reembolso del importe cuando se cancele un pedido ya pagado | Media |
| RF-31 | Sistema | Cancelar pedidos sin pagar | Cancelará automáticamente los pedidos que sigan pendientes de pago pasado un tiempo límite y liberará sus unidades | Media |
| RF-32 | Trabajador, Administrador | Consultar pedidos | Podrá visualizar todos los pedidos realizados por los clientes | Alta |
| RF-33 | Trabajador, Administrador | Cambiar estado de un pedido | Podrá modificar el estado de un pedido (Enviado, Entregado) | Alta |
| RF-34 | Sistema | Notificar cambio de estado | Enviará un email al cliente cuando cambie el estado de su pedido | Media |
| RF-35 | Administrador | Gestionar promociones | Podrá añadir, modificar o eliminar promociones, indicando su fecha de inicio y de fin | Alta |
| RF-36 | Trabajador, Administrador | Aplicar promociones | Podrá aplicar o retirar promociones de un producto | Alta |
| RF-37 | Sistema | Activar y retirar promociones | Aplicará cada promoción desde su fecha de inicio y la retirará automáticamente al llegar su fecha de fin | Alta |
| RF-38 | Sistema | Aplicar precios promocionales | Calculará el precio con descuento en catálogo, carrito y pedido mientras la promoción esté activa | Alta |
| RF-39 | Cliente | Valorar producto | Podrá escribir una reseña o puntuar un producto que le haya sido entregado | Media |
| RF-40 | Trabajador, Administrador | Moderar reseñas | Podrá eliminar reseñas | Media |
| RF-41 | Sistema | Calcular valoración media | Recalculará la puntuación media de un producto cuando se añada o elimine una reseña | Baja |
| RF-42 | Invitado, Cliente, Trabajador, Administrador | Consultar eventos | Podrá visualizar los eventos programados con su fecha, descripción, plazas disponibles y precio | Alta |
| RF-43 | Trabajador, Administrador | Gestionar eventos | Podrá crear, modificar o cancelar eventos, indicando fecha, descripción, aforo y precio | Alta |
| RF-44 | Cliente | Inscribirse en un evento | Podrá reservar plaza en un evento con plazas disponibles y pagar su inscripción si tiene precio | Alta |
| RF-45 | Sistema | Verificar plazas disponibles | Comprobará que quedan plazas al inscribirse y rechazará la inscripción si el evento está completo | Alta |
| RF-46 | Cliente | Cancelar inscripción | Podrá cancelar su inscripción hasta un plazo antes del evento; si estaba pagada, se le reembolsará | Media |
| RF-47 | Cliente | Consultar mis inscripciones | Podrá visualizar los eventos en los que está inscrito | Media |
| RF-48 | Trabajador, Administrador | Consultar asistentes de un evento | Podrá visualizar la lista de clientes inscritos en un evento | Media |
| RF-49 | Sistema | Gestionar cancelación de evento | Cuando se cancele un evento, notificará a los inscritos y reembolsará sus inscripciones pagadas | Media |
| RF-50 | Sistema | Recordar evento | Enviará un email de recordatorio a los inscritos antes del evento | Baja |
| RF-51 | Invitado, Cliente, Trabajador, Administrador | Consultar salas | Podrá visualizar las salas con su capacidad, tarifa y disponibilidad por fecha y franja horaria | Alta |
| RF-52 | Trabajador, Administrador | Gestionar salas | Podrá añadir, modificar o eliminar salas, y definir su capacidad, tarifa y horario de uso | Alta |
| RF-53 | Cliente | Reservar sala | Podrá reservar una sala disponible para una fecha y franja horaria, y pagar su tarifa | Alta |
| RF-54 | Sistema | Verificar disponibilidad de sala | Comprobará que la sala no esté ya reservada en esa franja y rechazará la reserva si hay solapamiento | Alta |
| RF-55 | Cliente | Cancelar reserva de sala | Podrá cancelar su reserva hasta un plazo antes de su inicio; si estaba pagada, se le reembolsará | Media |
| RF-56 | Cliente | Consultar mis reservas | Podrá visualizar sus reservas de sala con su estado | Media |
| RF-57 | Trabajador, Administrador | Consultar reservas de salas | Podrá visualizar todas las reservas de salas realizadas por los clientes | Alta |
| RF-58 | Sistema | Confirmar reservas tras el pago | Confirmará la inscripción o la reserva de sala cuando la pasarela confirme el pago | Alta |
| RF-59 | Sistema | Cancelar reservas sin pagar | Cancelará las inscripciones y reservas que sigan pendientes de pago pasado un tiempo límite y liberará su plaza o sala | Media |
| RF-60 | Sistema | Enviar confirmaciones por email | Enviará al cliente un email con los detalles de su inscripción o reserva, y de sus cambios o cancelaciones | Media |
| RF-61 | Cliente | Crear grupo | Podrá crear un grupo con nombre y descripción, y pasará a ser su propietario | Alta |
| RF-62 | Cliente (propietario) | Gestionar grupo | Podrá modificar los datos del grupo o eliminarlo | Media |
| RF-63 | Cliente (propietario) | Invitar a clientes | Podrá invitar a otros clientes registrados a unirse a su grupo | Alta |
| RF-64 | Cliente | Responder invitación | Podrá aceptar o rechazar una invitación a un grupo | Alta |
| RF-65 | Sistema | Notificar invitación | Avisará al cliente por email cuando reciba una invitación a un grupo | Baja |
| RF-66 | Cliente | Consultar mis grupos | Podrá visualizar los grupos a los que pertenece | Alta |
| RF-67 | Cliente (miembro) | Consultar contenido del grupo | Podrá visualizar los comentarios y las fotos de los grupos a los que pertenece | Alta |
| RF-68 | Cliente (miembro) | Publicar comentarios | Podrá escribir comentarios en el grupo | Alta |
| RF-69 | Cliente (miembro) | Subir fotos | Podrá subir fotos al grupo | Alta |
| RF-70 | Cliente (miembro) | Eliminar contenido propio | Podrá eliminar los comentarios y fotos que haya publicado | Media |
| RF-71 | Cliente (miembro) | Salir del grupo | Podrá abandonar un grupo | Media |
| RF-72 | Cliente (propietario) | Expulsar miembros | Podrá expulsar a un miembro de su grupo | Media |
| RF-73 | Cliente (miembro) | Reportar contenido | Podrá reportar un comentario o una foto de su grupo indicando el motivo | Alta |
| RF-74 | Trabajador, Administrador | Consultar reportes | Podrá visualizar los reportes pendientes con el contenido reportado y su motivo | Alta |
| RF-75 | Trabajador, Administrador | Resolver reporte | Podrá descartar un reporte o eliminar el contenido reportado | Alta |
| RF-76 | Sistema | Notificar resolución de reporte | Informará a quien reportó el contenido de que su reporte ha sido revisado | Baja |
| RF-77 | Trabajador, Administrador | Moderar grupos | Podrá acceder a cualquier grupo y eliminar comentarios, fotos o miembros, o eliminar el grupo completo | Alta |
| RF-78 | Administrador | Consultar estadísticas | Podrá visualizar las estadísticas de ventas de productos, inscripciones a eventos y reservas de salas | Baja |

## Requisitos no funcionales

| ID | Categoría | Requisito | Descripción | Prioridad |
| :---: | :---: | :---: | :---: | :---: |
| RNF-01 | Seguridad | Cifrado de contraseñas | Las contraseñas se almacenaran cifradas mediante hash seguro | Alta |
| RNF-02 | Seguridad | Comunicación segura | La comunicación entre cliente y servidor se realizará mediante https | Alta |
| RNF-03 | Seguridad | Control de roles | Cada funcionalidad sólo será accesible por los roles autorizados. Verificándose en cliente y en servidor | Alta |
| RNF-04 | Seguridad | Protección frente ataques | Se verificarán todas las entradas para evitar ataques cómo SQL inyeccion o XSS | Alta |
| RNF-05 | Seguridad | Contraseñas seguras | Las contraseñas de los usuarios deberán tenener una longitud mínima de 8 caractéres e incluirán números y letras | Media |
| RNF-06 | Seguridad | Datos de pago | La aplicación no almacenará datos de tarjetas | Alta |
| RNF-07 | Seguridad | Caducidad de sesión | La sesión se cerrará tras un período de inactividad de 15 minutos | Media |
| RNF-08 | Rendimiento | Tiempo de respuesta | Las páginas cargarán en menos de 3 segundos en condiciones normales de uso | Media |
| RNF-09 | Usabilidad | Adaptable | La interfaz de la aplicación presentará un diseño responsive, adaptándose a móvil, tablet y escritorio | Alta |
| RNF-10 | Usabilidad | Compatibilidad | La aplicación funcionará correctamente en las últimas versiones de los navegadores más populares (Chrome, Firefox, Edge y Safari) | Alta |
| RNF-11 | Usabilidad | Proceso de compra sencillo | El cliente podrá completar un pedido desde su carrito en un máximo de 4 pasos | Alta |
| RNF-12 | Usabilidad | Idiomas | La interfaz estará en español e inglés | Baja |
| RNF-13 | Fiabilidad | Integridad de pedidos y stock | El sistema se asegurará de que no se produzcan pedidos duplicados o stock negativo | Alta |
| RNF-14 | Fiabilidad | Copias de seguridad | Se realizarán copias de seguridad automáricas diariamente de la base de datos | Baja |
| RNF-15 | Fiabilidad | Registro de errores | El sistema registrará los errores que se produzcan | Baja |
| RNF-16 | Legal | Cookies | La aplicación pedirá la autorización del usuario para su uso | Alta |
| RNF-17 | Legal | Información legal de la tienda | Mostrará avisos legales, condiciones de venta y política de devoluciones y desistimiento | Alta |
| RNF-18 | Documentación | Manual de uso | La aplicación contará con un manual de uso para trabajadores y administradores | Baja |