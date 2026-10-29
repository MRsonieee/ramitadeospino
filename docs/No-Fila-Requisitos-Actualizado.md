# No Fila

## Documento de identificación y especificación inicial de requisitos

**Proyecto:** No Fila\
**Categoría:** SaaS · Gestión de negocios · Reservas · Transformación
digital\
**Tipo de solución:** Plataforma web adaptable y aplicaciones móviles
para Android e iOS\
**Estado del documento:** Propuesta inicial de requisitos, pendiente de
validación con usuarios\
**Versión:** 1.1\
**Fecha:** 29 de octubre de 2026\
**Preparado para:** Rama estudiantil IEEE

------------------------------------------------------------------------

## 1. Introducción

No Fila es una plataforma digital para que pequeños negocios de
diferentes sectores administren sus servicios, horarios, trabajadores y
citas desde un mismo sistema. Los clientes podrán descubrir negocios,
consultar servicios y reservar citas desde una página web o desde una
aplicación móvil.

La solución busca facilitar la digitalización de negocios como
barberías, peluquerías, centros de estética, spas, talleres de
reparación, consultorios y otros establecimientos que trabajan con citas
o turnos. La plataforma tendrá una estructura común y configurable para
adaptarse a las necesidades de cada negocio sin obligarlos a utilizar un
modelo de operación idéntico.

Este documento presenta una primera especificación de los requisitos de
No Fila. Los requisitos son propuestas iniciales y deberán validarse con
clientes potenciales, propietarios de negocios y trabajadores antes de
considerarse definitivos.

## 2. Contexto del proyecto

Muchos pequeños negocios coordinan sus citas mediante llamadas
telefónicas, mensajes de WhatsApp, redes sociales, agendas físicas o
anotaciones manuales. Estos métodos pueden ser suficientes cuando el
volumen de clientes es bajo, pero también pueden provocar reservas
duplicadas, citas olvidadas, errores de horario, dificultades para
reorganizar la agenda y pérdida de tiempo en tareas administrativas.

Los negocios de diferentes sectores también tienen necesidades
particulares. Por ejemplo, un servicio puede requerir un trabajador
específico, una duración determinada, una cabina, un equipo o un espacio
de atención. Una plataforma que no permita configurar estas condiciones
puede resultar poco útil para algunos establecimientos.

Por otra parte, los clientes necesitan consultar horarios y reservar sin
tener que llamar o escribir al negocio, y muchos prefieren hacerlo desde
el teléfono móvil. También necesitan descubrir establecimientos en su
barrio o en cualquier zona de una ciudad, comparar sus servicios y
reputación, y encontrar opciones fiables cuando visitan una ciudad nueva
o desean cambiar de negocio. Para los emprendimientos, aparecer en un
catálogo local con información y reseñas verificadas puede mejorar su
visibilidad y ayudarles a atraer nuevos clientes. Por ello, No Fila se plantea como una solución
multiplataforma: una aplicación web adaptable a distintos tamaños de
pantalla y aplicaciones móviles que faciliten las reservas, las
notificaciones y la consulta de citas.

## 3. Planteamiento del problema

Los pequeños negocios que administran citas o turnos pueden experimentar
dificultades para organizar su disponibilidad, coordinar a sus
trabajadores, evitar reservas superpuestas y mantener informados a sus
clientes. La utilización de canales dispersos y procesos manuales puede
ocasionar citas olvidadas, tiempos de espera innecesarios y
oportunidades de atención perdidas.

Además, los negocios de distintos sectores requieren reglas específicas
para la duración de los servicios, la asignación de trabajadores, la
disponibilidad de recursos y la reprogramación de citas. Al mismo
tiempo, los clientes necesitan una manera sencilla de consultar
servicios y reservar desde el dispositivo que prefieran.

Por tanto, se identifica la necesidad de una plataforma web y móvil
flexible y accesible que permita a pequeños negocios de distintos
sectores digitalizar la gestión de citas, publicar sus servicios y
horarios, administrar sus reservas desde un sistema centralizado y
aumentar su visibilidad mediante un catálogo de descubrimiento local y
un sistema confiable de calificaciones y reseñas de clientes.

## 4. Justificación

No Fila busca reducir la carga administrativa relacionada con la gestión
de citas y mejorar la experiencia tanto de los clientes como de los
negocios. La disponibilidad de canales web y móviles permitiría que los
clientes reserven desde un navegador o una aplicación, mientras que los
propietarios y trabajadores podrían consultar y gestionar las agendas
según sus permisos.

Una plataforma común también puede reducir la necesidad de que cada
negocio contrate o desarrolle una solución independiente. La
configuración por negocio permitiría incorporar diferentes sectores
gradualmente y validar las necesidades de cada uno sin reconstruir la
plataforma. Además, un catálogo por ciudad y barrio, acompañado de
calificaciones y reseñas vinculadas a citas completadas, puede ayudar a
los clientes a elegir con mayor confianza y ofrecer a los negocios una
vía adicional de promoción y reputación digital.

## 5. Objetivos

### 5.1. Objetivo general

Desarrollar una plataforma multiplataforma de gestión de citas y turnos
que permita a pequeños negocios de diferentes sectores administrar sus
servicios, horarios, trabajadores y reservas, facilitando a los clientes
el descubrimiento y la comparación de emprendimientos por ubicación y
reputación, así como la programación de citas mediante la web y
dispositivos móviles.

### 5.2. Objetivos específicos

1.  Permitir el registro y la configuración de diferentes tipos de
    negocios.
2.  Facilitar la publicación de servicios, precios, duración y
    disponibilidad.
3.  Permitir que los clientes consulten horarios y reserven citas desde
    la web o una aplicación móvil.
4.  Evitar reservas duplicadas mediante la validación de disponibilidad.
5.  Proporcionar herramientas para modificar, cancelar y consultar
    reservas.
6.  Incorporar notificaciones y recordatorios para clientes y negocios.
7.  Ofrecer un panel de administración para gestionar agendas,
    trabajadores y servicios.
8.  Diseñar una arquitectura que permita incorporar nuevos sectores
    comerciales sin reconstruir la plataforma.
9.  Mantener una experiencia coherente entre los canales web y móvil.
10. Permitir descubrir negocios por categoría, barrio y ciudad, con
    opciones de ordenamiento y filtrado útiles para el cliente.
11. Incorporar un sistema de calificaciones y reseñas asociado a citas
    completadas para promover confianza y reputación verificable.
12. Ayudar a los negocios a ganar visibilidad ante clientes potenciales
    y mostrar información clara sobre su valoración y número de reseñas.

## 6. Alcance

### 6.1. Incluido en el alcance inicial

-   Registro e inicio de sesión de clientes y propietarios.
-   Registro y configuración de negocios.
-   Clasificación de negocios por categoría.
-   Catálogo para descubrir emprendimientos por ciudad, barrio, categoría
    y servicios, con perfiles públicos de los establecimientos.
-   Visualización de calificación promedio y cantidad de reseñas.
-   Publicación, consulta y moderación básica de reseñas vinculadas a
    citas completadas.
-   Gestión de servicios, duración, precios y horarios.
-   Registro de trabajadores y asignación de servicios.
-   Consulta de disponibilidad y creación de reservas.
-   Confirmación, cancelación y reprogramación de citas.
-   Agenda para propietarios y trabajadores.
-   Notificaciones básicas, sujetas a la disponibilidad de los
    proveedores elegidos.
-   Interfaz web adaptable y aplicación móvil para clientes.
-   Control de acceso basado en roles.
-   Estadísticas básicas de reservas para los negocios.

### 6.2. Fuera del alcance inicial

Las siguientes funciones podrán evaluarse en versiones posteriores:

-   Pagos en línea y gestión de anticipos.
-   Comisiones automáticas y facturación avanzada.
-   Programas de fidelización y cupones.
-   Integraciones con múltiples plataformas de mensajería.
-   Gestión avanzada de inventario.
-   Analítica predictiva y recomendaciones automáticas.
-   Posicionamiento patrocinado o publicidad pagada de negocios.
-   Respuestas avanzadas del propietario a reseñas, programas de
    reputación y herramientas de marketing avanzadas.
-   Aplicaciones móviles nativas separadas para cada sistema operativo,
    si inicialmente se opta por una tecnología multiplataforma.

## 7. Actores del sistema

  -----------------------------------------------------------------------
  Actor                               Descripción y responsabilidades
  ----------------------------------- -----------------------------------
  Cliente                             Descubre y compara negocios por
                                      ubicación, categoría y reputación;
                                      consulta reseñas, agenda,
                                      reprograma o cancela sus propias
                                      citas y, tras una cita completada,
                                      puede publicar una reseña.

  Propietario del negocio             Registra el establecimiento y
                                      administra sus servicios,
                                      trabajadores, horarios y reservas.

  Trabajador o prestador del servicio Consulta su agenda y gestiona las
                                      citas que tiene asignadas, de
                                      acuerdo con sus permisos.

  Administrador de No Fila            Gestiona las cuentas de la
                                      plataforma, supervisa su
                                      funcionamiento y atiende
                                      incidencias.

  Servicio de notificaciones          Envía confirmaciones y
                                      recordatorios mediante los canales
                                      integrados.

  Moderador de contenido             Revisa reportes de reseñas o perfiles
                                      y gestiona contenido que incumpla
                                      las políticas de la plataforma.

  Proveedor de autenticación, si      Apoya la autenticación de usuarios
  aplica                              cuando se utiliza un servicio
                                      externo.
  -----------------------------------------------------------------------

## 8. Requisitos funcionales

Los requisitos funcionales describen las acciones y servicios que debe
proporcionar el sistema.

  -----------------------------------------------------------------------
  Código                  Nombre                  Descripción
  ----------------------- ----------------------- -----------------------
  RF-01                   Registro de usuarios    El sistema debe
                                                  permitir el registro e
                                                  inicio de sesión de
                                                  clientes y propietarios
                                                  de negocios.

  RF-02                   Registro de negocios    El sistema debe
                                                  permitir que un
                                                  propietario registre un
                                                  establecimiento y
                                                  configure su
                                                  información comercial.

  RF-03                   Clasificación por       El sistema debe
                          sector                  permitir categorizar
                                                  los negocios por tipo
                                                  de servicio, sin
                                                  limitarse a un único
                                                  sector comercial.

  RF-04                   Perfil del negocio      El sistema debe
                                                  permitir publicar el
                                                  nombre, descripción,
                                                  ubicación, horarios,
                                                  medios de contacto y
                                                  demás información
                                                  autorizada del
                                                  establecimiento.

  RF-05                   Gestión de servicios    El propietario debe
                                                  poder crear, modificar
                                                  y desactivar servicios,
                                                  indicando su duración,
                                                  precio y descripción.

  RF-06                   Gestión de trabajadores El sistema debe
                                                  permitir registrar
                                                  trabajadores y
                                                  asociarlos con los
                                                  servicios que pueden
                                                  prestar.

  RF-07                   Configuración de        El propietario debe
                          horarios                poder definir horarios
                                                  de atención, descansos,
                                                  días no laborables y
                                                  excepciones de
                                                  calendario.

  RF-08                   Consulta de             El cliente debe poder
                          disponibilidad          consultar horarios
                                                  disponibles para un
                                                  servicio, trabajador o
                                                  establecimiento.

  RF-09                   Reserva de citas        El sistema debe
                                                  permitir que un cliente
                                                  seleccione un servicio,
                                                  un horario disponible y
                                                  confirme una reserva
                                                  desde la web o la
                                                  aplicación móvil.

  RF-10                   Prevención de           El sistema debe
                          duplicados              verificar la
                                                  disponibilidad antes de
                                                  confirmar una cita y
                                                  evitar reservas
                                                  incompatibles sobre el
                                                  mismo recurso.

  RF-11                   Confirmación de reserva El sistema debe mostrar
                                                  los datos de la cita y
                                                  confirmar si fue
                                                  registrada
                                                  correctamente.

  RF-12                   Modificación de citas   El sistema debe
                                                  permitir reprogramar
                                                  citas de acuerdo con
                                                  las reglas definidas
                                                  por el negocio.

  RF-13                   Cancelación de citas    El sistema debe
                                                  permitir cancelar
                                                  reservas conforme a las
                                                  políticas de
                                                  cancelación
                                                  establecidas.

  RF-14                   Agenda del negocio      El propietario debe
                                                  poder consultar las
                                                  citas por fecha,
                                                  trabajador, servicio y
                                                  estado.

  RF-15                   Recordatorios           El sistema debe
                                                  permitir enviar
                                                  recordatorios de las
                                                  citas mediante los
                                                  canales de notificación
                                                  habilitados.

  RF-16                   Historial de reservas   El cliente y el negocio
                                                  deben poder consultar
                                                  el historial de las
                                                  citas a las que tengan
                                                  acceso autorizado.

  RF-17                   Gestión de ausencias    El negocio debe poder
                                                  registrar bloqueos
                                                  temporales de
                                                  disponibilidad,
                                                  vacaciones o ausencias
                                                  de trabajadores.

  RF-18                   Gestión de recursos     El sistema debe
                                                  permitir configurar
                                                  recursos compartidos
                                                  cuando un servicio
                                                  requiera instalaciones,
                                                  equipos o espacios
                                                  específicos.

  RF-19                   Búsqueda de negocios    El cliente debe poder
                                                  buscar negocios por
                                                  nombre, categoría,
                                                  ubicación y servicios
                                                  ofrecidos.

  RF-20                   Gestión de permisos     El sistema debe
                                                  diferenciar los
                                                  permisos de clientes,
                                                  trabajadores,
                                                  propietarios y
                                                  administradores de la
                                                  plataforma.

  RF-21                   Panel de administración El propietario debe
                                                  disponer de un panel
                                                  para gestionar su
                                                  negocio sin acceder a
                                                  la información privada
                                                  de otros
                                                  establecimientos.

  RF-22                   Estadísticas básicas    El sistema debe
                                                  permitir consultar
                                                  métricas como número de
                                                  citas, cancelaciones y
                                                  servicios más
                                                  reservados, según los
                                                  datos disponibles.

  RF-23                   Acceso web              El sistema debe
                                                  permitir utilizar las
                                                  funciones aplicables
                                                  desde una interfaz web
                                                  adaptable a equipos de
                                                  escritorio, tabletas y
                                                  móviles.

  RF-24                   Acceso mediante         El sistema debe
                          aplicación móvil        permitir que los
                                                  clientes consulten
                                                  negocios, reserven
                                                  citas y administren sus
                                                  reservas desde una
                                                  aplicación móvil
                                                  compatible.

  RF-25                   Sincronización de       Los cambios de una cita
                          reservas                realizados desde la web
                                                  o la aplicación móvil
                                                  deben reflejarse en los
                                                  demás canales una vez
                                                  confirmados por el
                                                  servidor.

  RF-26                   Notificaciones móviles  La aplicación móvil
                                                  debe poder recibir
                                                  notificaciones push
                                                  cuando el usuario haya
                                                  concedido los permisos
                                                  necesarios y el
                                                  servicio esté
                                                  disponible.

  RF-27                   Gestión de sesión       El usuario debe poder
                                                  cerrar sesión y
                                                  gestionar el acceso a
                                                  su cuenta desde los
                                                  canales compatibles.

  RF-28                   Actualización de la     La aplicación móvil
                          aplicación              debe informar o manejar
                                                  de forma segura los
                                                  cambios de versión que
                                                  afecten su
                                                  compatibilidad con los
                                                  servicios de No Fila.
  RF-29                   Exploración por ubicación El cliente debe poder descubrir negocios por ciudad y, cuando exista información suficiente, por barrio o zona; la búsqueda no debe limitarse a su ubicación actual.

  RF-30                   Filtros y ordenamiento     El cliente debe poder filtrar los negocios por categoría, servicios y ubicación, y ordenar los resultados por calificación, cantidad de reseñas o cercanía cuando la ubicación esté disponible.

  RF-31                   Perfil público ampliado    El sistema debe mostrar en el perfil de cada negocio su descripción, dirección o zona, servicios, precios publicados, horarios, calificación promedio y cantidad de reseñas.

  RF-32                   Calificar una experiencia  Un cliente autenticado debe poder calificar con una escala definida (por ejemplo, de 1 a 5 estrellas) una cita que figure como completada.

  RF-33                   Publicar reseña            El cliente debe poder escribir una reseña asociada a una cita completada, de acuerdo con las reglas de publicación de la plataforma.

  RF-34                   Control de reseñas         El sistema debe impedir más de una reseña activa por cita completada y permitir reportar contenido abusivo, falso o inapropiado para su revisión.

  RF-35                   Consultar reputación       El sistema debe calcular y mostrar la calificación promedio y el número de reseñas de cada negocio, actualizando los datos cuando se publique, modifique o retire una reseña válida.

  RF-36                   Negocios mejor valorados   El sistema debe permitir consultar negocios destacados por calificación dentro de una categoría y ubicación elegidas, mostrando también la cantidad de reseñas para aportar contexto.

  RF-37                   Gestión de reseñas         El administrador autorizado debe poder revisar reportes y moderar reseñas que incumplan las políticas, conservando trazabilidad de las acciones de moderación.
  -----------------------------------------------------------------------

## 9. Requisitos no funcionales

Los requisitos no funcionales establecen las condiciones de calidad,
seguridad y rendimiento que debe cumplir la plataforma.

  -----------------------------------------------------------------------
  Código                  Categoría               Requisito no funcional
  ----------------------- ----------------------- -----------------------
  RNF-01                  Rendimiento             Las consultas
                                                  habituales de
                                                  disponibilidad deben
                                                  responder en un tiempo
                                                  objetivo de dos
                                                  segundos o menos bajo
                                                  la carga de referencia
                                                  definida para las
                                                  pruebas.

  RNF-02                  Consistencia            La confirmación de una
                                                  reserva debe realizarse
                                                  de forma que dos
                                                  clientes no puedan
                                                  obtener la misma franja
                                                  de tiempo para un
                                                  recurso incompatible.

  RNF-03                  Seguridad               El sistema debe
                                                  proteger las cuentas y
                                                  restringir el acceso a
                                                  las funciones según el
                                                  rol del usuario.

  RNF-04                  Privacidad              Los datos personales de
                                                  los clientes solo deben
                                                  ser accesibles para
                                                  usuarios autorizados y
                                                  utilizarse conforme a
                                                  la finalidad informada.

  RNF-05                  Usabilidad              El proceso de reserva
                                                  debe presentar pasos
                                                  claros para elegir un
                                                  servicio, consultar
                                                  horarios y confirmar
                                                  una cita.

  RNF-06                  Compatibilidad web      La interfaz web debe
                                                  funcionar en las
                                                  versiones de
                                                  navegadores modernos
                                                  que se definan como
                                                  compatibles.

  RNF-07                  Compatibilidad móvil    La aplicación móvil
                                                  debe ser compatible con
                                                  las versiones de
                                                  Android y/o iOS que se
                                                  definan para cada
                                                  lanzamiento.

  RNF-08                  Diseño adaptable        La interfaz web debe
                                                  adaptarse a distintos
                                                  tamaños de pantalla sin
                                                  perder las funciones
                                                  esenciales.

  RNF-09                  Escalabilidad           La arquitectura debe
                                                  permitir incorporar
                                                  nuevos negocios,
                                                  trabajadores, servicios
                                                  y sectores sin crear
                                                  una aplicación separada
                                                  para cada uno.

  RNF-10                  Disponibilidad          El sistema debe
                                                  gestionar fallos de los
                                                  servicios de
                                                  notificación sin perder
                                                  las reservas
                                                  confirmadas.

  RNF-11                  Mantenibilidad          Los módulos de
                                                  reservas, servicios,
                                                  usuarios,
                                                  notificaciones y
                                                  estadísticas deben
                                                  poder mantenerse de
                                                  manera independiente.

  RNF-12                  Integridad              Las citas deben
                                                  conservar relaciones
                                                  válidas con el cliente,
                                                  negocio, servicio,
                                                  trabajador y recursos
                                                  que correspondan.

  RNF-13                  Recuperación            El sistema debe contar
                                                  con procedimientos de
                                                  copia de seguridad y
                                                  recuperación de datos
                                                  acordes con los
                                                  objetivos de
                                                  continuidad
                                                  establecidos.

  RNF-14                  Configurabilidad        Las reglas de duración,
                                                  horarios, cancelación y
                                                  asignación de
                                                  trabajadores deben
                                                  poder ajustarse por
                                                  negocio sin modificar
                                                  el código fuente.

  RNF-15                  Consistencia entre      La web y la aplicación
                          canales                 móvil deben presentar
                                                  estados coherentes de
                                                  las reservas,
                                                  utilizando el servidor
                                                  como fuente de verdad.

  RNF-16                  Accesibilidad           Las interfaces deben
                                                  ofrecer controles
                                                  comprensibles,
                                                  navegación por teclado
                                                  en la web y
                                                  compatibilidad con las
                                                  funciones de
                                                  accesibilidad
                                                  disponibles en los
                                                  sistemas móviles.

  RNF-17                  Protección de           La comunicación entre
                          comunicaciones          clientes, aplicaciones
                                                  y servicios debe
                                                  utilizar canales
                                                  cifrados, como
                                                  HTTPS/TLS.

  RNF-18                  Gestión de errores      La plataforma debe
                                                  mostrar mensajes
                                                  comprensibles cuando
                                                  falle una operación y
                                                  evitar informar una
                                                  reserva como confirmada
                                                  si el servidor no la ha
                                                  registrado.
  RNF-19                  Calidad de búsqueda       Las búsquedas por categoría y ubicación deben ofrecer resultados consistentes y comprensibles; la plataforma debe indicar cuando no existan resultados para los filtros seleccionados.

  RNF-20                  Transparencia de           La calificación promedio debe mostrarse junto con la cantidad de reseñas; el ordenamiento por valoración no debe ocultar ese contexto.
                          calificaciones

  RNF-21                  Integridad de reseñas     Las reseñas deben vincularse a citas completadas verificables y el sistema debe aplicar controles contra duplicados y modificaciones no autorizadas.

  RNF-22                  Moderación y seguridad    La plataforma debe ofrecer mecanismos para reportar reseñas y restringir contenido que infrinja sus políticas, respetando la privacidad y manteniendo registros de moderación.
  -----------------------------------------------------------------------

## 10. Restricciones y reglas de negocio

1.  Cada negocio debe administrar su propia información, servicios,
    trabajadores y agenda.
2.  La duración de cada cita dependerá del servicio seleccionado y de la
    configuración del negocio.
3.  No se podrán confirmar citas que se superpongan para un mismo
    trabajador o recurso exclusivo.
4.  Las citas deberán respetar los horarios de atención, los bloqueos de
    agenda y los periodos de descanso configurados.
5.  Las políticas de cancelación y reprogramación deberán informarse al
    cliente antes de confirmar la reserva.
6.  La plataforma no debe exigir que todos los negocios trabajen de la
    misma manera; cada sector debe poder configurar sus necesidades.
7.  Las notificaciones por correo, SMS o mensajería dependerán de la
    disponibilidad e integración de los proveedores correspondientes.
8.  La aplicación móvil necesitará conexión a internet para confirmar
    cambios de disponibilidad y registrar reservas en el servidor. La
    información guardada localmente no debe presentarse como una reserva
    confirmada.
9.  Las notificaciones push dependerán de los permisos concedidos por el
    usuario, del dispositivo y de los servicios de entrega.
10. Los datos personales deberán tratarse de acuerdo con la legislación
    aplicable y las políticas de privacidad comunicadas a los usuarios.
11. Las funciones de pagos en línea, anticipos, facturación y comisiones
    comerciales no serán obligatorias en la primera versión, salvo que
    se incorporen expresamente al alcance.
12. Las publicaciones de negocios y servicios estarán sujetas a las
    reglas de uso de la plataforma.
13. Solo los clientes autenticados con una cita marcada como completada
    podrán publicar una reseña para esa cita.
14. Se permitirá como máximo una reseña activa por cita; cualquier
    edición posterior deberá seguir la política de reseñas definida.
15. Las reseñas deben reflejar experiencias reales y no podrán contener
    amenazas, datos personales de terceros, spam ni contenido ilegal.
16. Los usuarios podrán reportar reseñas; la plataforma podrá ocultar o
    retirar contenido tras una revisión conforme a sus políticas.
17. La calificación promedio se mostrará junto con el número de reseñas;
    una puntuación alta basada en pocas reseñas no se presentará sin ese
    contexto.
18. La búsqueda por ciudad o barrio no dependerá exclusivamente del
    GPS del usuario: deberá permitir elegir manualmente una ubicación.
19. La posición orgánica de los resultados debe basarse en criterios
    explicables, como filtros elegidos, valoración, número de reseñas y
    ubicación; cualquier promoción pagada futura deberá identificarse.

## 11. Criterios de aceptación iniciales

-   **CA-01:** un propietario debe poder registrar su negocio y publicar
    al menos un servicio.
-   **CA-02:** un cliente debe poder consultar los horarios disponibles
    de ese servicio desde la web o la aplicación móvil.
-   **CA-03:** una reserva confirmada debe aparecer en la agenda del
    negocio y en la cuenta del cliente.
-   **CA-04:** si dos clientes intentan reservar simultáneamente un
    mismo horario incompatible, el sistema debe confirmar como máximo
    una reserva.
-   **CA-05:** al cancelar una cita, su estado debe actualizarse y el
    horario debe liberarse según las reglas del negocio.
-   **CA-06:** un trabajador no debe poder consultar ni modificar las
    agendas privadas de negocios a los que no esté autorizado.
-   **CA-07:** una reserva realizada desde la web debe ser visible en la
    aplicación móvil del mismo usuario, y viceversa, después de que el
    servidor confirme la operación.
-   **CA-08:** si no hay conexión a internet, la aplicación móvil no
    debe mostrar una nueva reserva como confirmada sin respuesta
    satisfactoria del servidor.
-   **CA-09:** si las notificaciones están desactivadas en el
    dispositivo, el usuario debe poder consultar el estado de sus
    reservas dentro de la aplicación.
-   **CA-10:** al registrar un nuevo sector comercial, el administrador
    debe poder configurar sus categorías y servicios sin necesidad de
    crear una aplicación independiente.
-   **CA-11:** el cliente puede seleccionar Santa Marta u otra ciudad y
    consultar negocios de esa ciudad, sin limitarse a su barrio actual.
-   **CA-12:** el cliente puede filtrar los negocios por categoría y
    servicio, y consultar el perfil de cada establecimiento.
-   **CA-13:** el perfil del negocio muestra su calificación promedio y
    la cantidad total de reseñas publicadas.
-   **CA-14:** un cliente puede publicar una reseña si su cita está
    completada; el sistema rechaza una reseña asociada a una cita no
    completada o una segunda reseña activa para la misma cita.
-   **CA-15:** después de publicar una reseña válida, la calificación
    promedio y el número de reseñas del negocio se actualizan.
-   **CA-16:** los resultados mejor valorados muestran también la cantidad
    de reseñas para que el cliente pueda interpretar la puntuación.
-   **CA-17:** un usuario puede reportar una reseña y un moderador
    autorizado puede revisarla sin acceder a datos privados innecesarios.

## 12. Riesgos, supuestos y preguntas pendientes

### 12.1. Riesgos iniciales

-   Dificultad para conseguir que los negocios registren y mantengan
    actualizada su información.
-   Competencia con herramientas de agenda y reserva que ya utilizan
    algunos establecimientos.
-   Costos asociados al envío de notificaciones y al alojamiento de la
    plataforma.
-   Conflictos de disponibilidad si no se implementa correctamente la
    confirmación transaccional de reservas.
-   Diferencias de funcionamiento y mantenimiento entre versiones de
    Android, iOS y navegadores.
-   Tratamiento inadecuado de datos personales si no se definen
    controles y políticas desde el inicio.
-   Reseñas falsas, campañas de calificaciones manipuladas o conflictos
    entre clientes y negocios.
-   Pocos negocios registrados al inicio, lo que podría producir
    catálogos incompletos o poca utilidad en algunas zonas.
-   Disputas por la moderación de reseñas negativas y necesidad de
    definir criterios transparentes de revisión.

### 12.2. Supuestos iniciales

-   Los negocios podrán definir al menos un servicio y un horario de
    atención.
-   Los clientes tendrán acceso a internet al momento de confirmar una
    reserva.
-   La plataforma utilizará un servidor central como fuente oficial del
    estado de las citas.
-   La primera versión podrá comenzar con un número limitado de sectores
    comerciales y ampliar su cobertura después de validarse.

### 12.3. Preguntas para validar con usuarios

1.  ¿Qué tipos de negocio tienen mayor necesidad de gestionar citas
    digitalmente?
2.  ¿Los propietarios prefieren administrar sus agendas desde la web, el
    móvil o ambos?
3.  ¿Qué canales de recordatorio utilizan actualmente los negocios y sus
    clientes?
4.  ¿Qué políticas de cancelación y reprogramación necesitan?
5.  ¿Los clientes necesitan reservar sin crear una cuenta?
6.  ¿Los negocios requieren varios trabajadores, sucursales o recursos
    compartidos?
7.  ¿Estarían dispuestos los negocios a pagar por la plataforma? ¿Qué
    modelo de precio aceptarían?
8.  ¿Qué funciones deben incluirse en la primera versión para que los
    negocios quieran probarla?
9.  ¿Qué categorías y zonas geográficas deben priorizarse para que el
    catálogo local sea útil desde el lanzamiento?
10. ¿Qué escala de valoración y qué política de edición, respuesta y
    moderación de reseñas resultan adecuadas?
11. ¿Qué información de ubicación desea compartir el cliente y qué
    controles necesita para buscar manualmente por ciudad o barrio?

## 13. Alcance recomendado para el producto mínimo viable (MVP)

La primera versión de No Fila debería concentrarse en un flujo completo
y confiable de reserva:

1.  Registro e inicio de sesión.
2.  Creación del perfil de un negocio.
3.  Publicación de servicios, duración, precios y horarios.
4.  Consulta de disponibilidad.
5.  Reserva, confirmación y cancelación de citas.
6.  Agenda básica para el propietario.
7.  Interfaz web adaptable y aplicación móvil para clientes.
8.  Sincronización de reservas entre canales.
9.  Confirmaciones dentro de la plataforma y un canal básico de
    recordatorios.
10. Control de permisos y protección de datos.
11. Catálogo de negocios por ciudad y barrio, con filtros por categoría
    y servicio.
12. Perfiles públicos de negocios con calificación promedio y número
    de reseñas.
13. Reseñas y calificaciones de clientes asociadas a citas completadas,
    con reporte y moderación básica.

Se recomienda iniciar con sectores como barberías, centros de estética y
servicios de mantenimiento o reparación. Estos permitirían validar
diferentes necesidades sin intentar cubrir todos los sectores desde el
primer día.

Las funciones de pagos, programas de fidelización, múltiples sucursales,
analítica avanzada, publicidad pagada y automatizaciones pueden
incorporarse en fases posteriores. El catálogo y las reseñas básicas se
consideran parte del valor central del MVP, aunque su cobertura inicial
puede limitarse a las ciudades y negocios participantes en la prueba.

## 14. Consideraciones de arquitectura

Como punto de partida, se recomienda una arquitectura en la que la web y
la aplicación móvil consuman una API compartida. El servidor central
gestionaría la autenticación, los negocios, los servicios, los horarios
y las reservas, y una base de datos central conservaría el estado
oficial de las citas.

Esta arquitectura ayuda a mantener la coherencia entre canales y evita
que la aplicación móvil y la web mantengan agendas independientes. El
servidor también deberá gestionar el catálogo de negocios, las ubicaciones,
las valoraciones, las reseñas y los reportes de moderación. Las búsquedas
por ciudad y barrio deberán funcionar aunque el usuario elija la ubicación
manualmente; el GPS podrá utilizarse como opción, solo con permiso del
usuario. Las reseñas deberán relacionarse con citas completadas y los
promedios deberán calcularse desde las reseñas válidas, no desde valores
introducidos libremente por el negocio. La
tecnología concreta deberá elegirse después de evaluar los conocimientos
del equipo, los costos, los requisitos de publicación y las necesidades
de mantenimiento.

## 15. Conclusión

No Fila propone una solución multiplataforma para simplificar la gestión
de citas en pequeños negocios de diferentes sectores y, al mismo tiempo,
facilitar que los clientes descubran emprendimientos por ciudad o barrio,
comparen sus servicios y reputación y compartan reseñas basadas en
experiencias reales. Al combinar catálogo local, reputación verificable,
interfaz web y aplicación móvil, la plataforma busca ayudar a los clientes
a elegir con mayor confianza y ofrecer a los negocios una vía adicional
para ganar visibilidad y atraer nuevos clientes.

La viabilidad del proyecto dependerá de validar las necesidades de los
negocios, mantener una gestión consistente de la disponibilidad y
proteger los datos de los usuarios. Por ello, se recomienda desarrollar
primero un MVP acotado, realizar pruebas con negocios reales y utilizar
sus resultados para priorizar las siguientes funcionalidades.

------------------------------------------------------------------------

**Nota de documentación:** esta especificación es una propuesta inicial.
Los requisitos, las metas de rendimiento, las restricciones y el alcance
deberán revisarse con las partes interesadas antes de aprobar una
versión definitiva.
