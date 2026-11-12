# No Fila

**Documento de especificación de requisitos**

| | |
|---|---|
| **Proyecto** | No Fila |
| **Tipo de solución** | Aplicación móvil para Android orientada a la gestión de citas en barberías |
| **Versión** | 2.0 |
| **Fecha** | 12 de noviembre de 2026 |
| **Preparado para** | Rama estudiantil IEEE |
| **Estado** | Propuesta pendiente de validación con usuarios |

**Keywords:** No Fila, gestión de citas, barberías, aplicación móvil, Android, Kotlin, Jetpack Compose, Firebase, reservas, reseñas, ingeniería de requisitos, Santa Marta.

---

## 1. Introducción

No Fila es una aplicación móvil para Android que permite a los clientes de barberías agendar sus citas sin depender de llamadas o mensajes al número personal del barbero. Los barberos y propietarios administran sus servicios, horarios y agenda desde la misma aplicación, y los clientes pueden consultar las reseñas de otros usuarios antes de elegir. Este documento especifica los requisitos de su primera versión, orientada a barberías de Santa Marta.

## 2. Contexto del problema

Muchas barberías coordinan sus citas mediante llamadas, mensajes de WhatsApp, redes sociales o agendas físicas. Estos métodos pueden funcionar con pocos clientes, pero provocan reservas duplicadas, citas olvidadas, errores de horario y pérdida de tiempo. Además, los barberos reciben mensajes de clientes en sus números personales a cualquier hora, y los clientes no tienen una forma sencilla de conocer la reputación de una barbería antes de visitarla.

## 3. Planteamiento del problema

Las barberías que administran citas de forma manual tienen dificultades para organizar la disponibilidad de sus barberos, evitar reservas superpuestas y mantener informados a sus clientes. Los clientes, por su parte, necesitan una manera sencilla de reservar y de elegir con confianza. Se identifica entonces la necesidad de una aplicación móvil que centralice la gestión de citas de las barberías y ofrezca reseñas verificables de clientes.

## 4. Justificación

No Fila busca reducir la carga administrativa de las barberías y mejorar la experiencia de sus clientes. Separar la gestión de citas de los números personales de los barberos ordena el trabajo, y las reseñas vinculadas a citas completadas ayudan a los clientes a elegir y a las barberías a construir una reputación verificable.

## 5. Objetivos

### 5.1. Objetivo general

**Implementar** una aplicación móvil Android que permita gestionar las citas de barberías en Santa Marta.

### 5.2. Objetivos específicos

1. **Diseñar** la base de datos y la arquitectura de la aplicación para almacenar barberías, servicios, horarios, citas y reseñas.
2. **Implementar** los módulos de reserva de citas y de reseñas, evitando que dos clientes tomen el mismo horario.
3. **Evaluar** el funcionamiento de la aplicación mediante pruebas con barberos y clientes reales.

## 6. Alcance

**Incluido en la primera versión:**

1. **Gestión de la barbería:** registro del negocio, servicios (duración y precio), barberos y horarios.
2. **Reserva de citas:** consulta de disponibilidad, reserva, cancelación y reprogramación, con validación para evitar horarios duplicados.
3. **Reseñas y reputación:** calificación y comentario posteriores a una cita completada.
4. **Agenda y recordatorios:** agenda para barberos y propietarios, y recordatorios de citas.

**Fuera del alcance (trabajo futuro):** pagos en línea, programas de fidelización, versión para iOS, versión web y otros sectores comerciales.

## 7. Actores del sistema

| Actor | Responsabilidades |
|---|---|
| **Cliente** | Busca barberías, agenda, cancela y reprograma citas, y deja reseñas. |
| **Propietario** | Registra la barbería y administra sus servicios, barberos y horarios. |
| **Barbero** | Consulta su agenda, gestiona sus citas y las marca como completadas. |

## 8. Herramientas y tecnologías

| Necesidad | Herramienta |
|---|---|
| Lenguaje | Kotlin |
| Interfaz | Jetpack Compose |
| Entorno de desarrollo | Android Studio |
| Autenticación | Firebase Authentication |
| Base de datos | Cloud Firestore |
| Recordatorios | WorkManager |
| Control de versiones | Git y GitHub |
| Diseño de pantallas | Figma |

## 9. Requisitos funcionales

| Código | Requisito |
|---|---|
| **RF-01** | **Autenticación y roles:** el sistema debe permitir registrarse, iniciar y cerrar sesión, diferenciando los roles cliente, propietario y barbero. |
| **RF-02** | **Gestión de la barbería:** el propietario debe poder registrar su barbería, sus servicios (duración y precio) y a sus barberos. |
| **RF-03** | **Horarios y ausencias:** el propietario y el barbero deben poder definir horarios de atención, descansos y días no disponibles. |
| **RF-04** | **Búsqueda de barberías:** el cliente debe poder buscar barberías por nombre, barrio o servicio, ver su perfil y ordenarlas por calificación. |
| **RF-05** | **Reserva de citas:** el cliente debe poder consultar horarios disponibles y reservar una cita, y el sistema debe confirmarla solo si el horario sigue libre. |
| **RF-06** | **Gestión de citas:** el cliente debe poder cancelar, reprogramar y consultar su historial; el barbero y el propietario deben poder ver la agenda, y el barbero marcar una cita como completada. |
| **RF-07** | **Recordatorios:** el sistema debe notificar al cliente antes de su cita. |
| **RF-08** | **Reseñas y reputación:** el cliente debe poder calificar (1 a 5) y comentar una cita completada; el sistema debe actualizar el promedio y ocultar automáticamente una reseña que acumule varios reportes. |

## 10. Requisitos no funcionales

| Código | Categoría | Requisito |
|---|---|---|
| **RNF-01** | Rendimiento | La consulta de horarios debe responder en 2 segundos o menos. |
| **RNF-02** | Integridad de reservas | El sistema no debe permitir dos citas en el mismo horario para un barbero; el servidor es la única fuente de verdad. |
| **RNF-03** | Seguridad | Los datos deben viajar cifrados (HTTPS/TLS) y cada rol solo debe acceder a lo que le corresponde. |
| **RNF-04** | Privacidad | Los datos personales deben tratarse conforme a la Ley 1581 de 2012 y ser visibles solo para usuarios autorizados. |
| **RNF-05** | Usabilidad y accesibilidad | Reservar debe tomar máximo 4 pasos, con textos legibles y compatibilidad con las funciones de accesibilidad de Android. |
| **RNF-06** | Compatibilidad | La app debe funcionar en Android 8.0 o superior. |
| **RNF-07** | Disponibilidad y errores | Sin internet, la app no debe mostrar una reserva como confirmada; ante un fallo debe mostrar un mensaje claro y no perder reservas ya confirmadas. |
| **RNF-08** | Mantenibilidad y escalabilidad | El código debe organizarse en módulos independientes (usuarios, citas, reseñas) para poder añadir otros sectores a futuro. |
| **RNF-09** | Transparencia de reseñas | El promedio debe mostrarse junto con la cantidad de reseñas y calcularse solo desde reseñas válidas. |

> Los valores numéricos (2 segundos, 4 pasos, Android 8.0) son de referencia y deben confirmarse en las pruebas.

## 11. Reglas de negocio

1. **RN-01:** No se pueden confirmar citas que se superpongan para un mismo barbero, ni fuera de sus horarios de atención, descansos o ausencias.
2. **RN-02:** La duración de cada cita depende del servicio seleccionado.
3. **RN-03:** La política de cancelación y reprogramación (por ejemplo, un mínimo de 2 horas de anticipación) se informa al cliente antes de confirmar la reserva.
4. **RN-04:** Solo un cliente con una cita marcada como completada por el barbero puede publicar una reseña, y solo una por cita. Las reseñas no pueden contener amenazas, datos personales de terceros, spam ni contenido ilegal.
5. **RN-05:** Una reseña que reciba 3 reportes se oculta automáticamente (valor de referencia). El promedio siempre se muestra junto con el número de reseñas.
6. **RN-06:** Cada barbería administra únicamente su propia información, servicios, barberos y agenda.
7. **RN-07:** Reservar requiere conexión a internet; la información guardada localmente no se presenta como reserva confirmada.

## 12. Criterios de aceptación

| Código | Requisito | Criterio |
|---|---|---|
| **CA-01** | RF-02 | Un propietario puede registrar su barbería y publicar al menos un servicio con duración y precio. |
| **CA-02** | RF-03, RF-05 | Un cliente ve los horarios disponibles de un servicio, reserva, y la cita aparece en la agenda del barbero. |
| **CA-03** | RNF-02 | Si dos clientes reservan a la vez el mismo horario, el sistema confirma como máximo una reserva. |
| **CA-04** | RF-06 | Al cancelar una cita, su estado se actualiza y el horario queda libre. |
| **CA-05** | RNF-07 | Sin internet, la app no muestra una nueva reserva como confirmada. |
| **CA-06** | RF-01, RNF-03 | Un barbero no puede consultar ni modificar la agenda de otra barbería. |
| **CA-07** | RF-07 | El cliente recibe un recordatorio antes de su cita. |
| **CA-08** | RF-08, RNF-09 | El sistema rechaza una reseña de una cita no completada o una segunda reseña de la misma cita; al publicar una reseña válida, el promedio y la cantidad se actualizan. |
| **CA-09** | RF-04 | El cliente puede filtrar barberías por barrio y servicio, y ver el perfil con su calificación y número de reseñas. |

## 13. Riesgos, supuestos y preguntas pendientes

### 13.1. Riesgos

1. Que las barberías no adopten la app o no mantengan su información actualizada.
2. Reservas duplicadas si la validación de disponibilidad falla.
3. Reseñas falsas o manipuladas.
4. Poca experiencia del equipo con Kotlin y Firebase (curva de aprendizaje).
5. Que el uso supere los límites del plan gratuito de Firebase.

### 13.2. Supuestos

1. Propietarios y barberos cuentan con un dispositivo Android e internet.
2. Firebase actúa como fuente central del estado de las citas.
3. Se iniciará con un número reducido de barberías de Santa Marta.

### 13.3. Preguntas por validar

1. ¿Qué política de cancelación y reprogramación necesitan las barberías?
2. ¿Las barberías tienen varios barberos o trabajan de forma individual?
3. ¿Los barberos y propietarios usan Android?
4. ¿Estarían dispuestas las barberías a pagar por la aplicación en el futuro?

## 14. Alcance del producto mínimo viable (MVP)

La primera versión se concentra en un flujo completo y confiable:

1. Registro, inicio de sesión y roles (RF-01).
2. Perfil de la barbería con servicios, barberos y horarios (RF-02, RF-03).
3. Búsqueda, disponibilidad y reserva de citas sin duplicados (RF-04, RF-05).
4. Cancelación, reprogramación y agenda (RF-06).
5. Reseñas básicas con moderación automática (RF-08).

Los recordatorios (RF-07) se incorporan cuando el flujo de reserva esté estable.

## 15. Consideraciones de arquitectura

La aplicación Android (Kotlin y Jetpack Compose) se organiza con el patrón **MVVM** y se conecta directamente a los servicios de Firebase:

```
App Android (Kotlin + Jetpack Compose)
        │
        ├── Firebase Authentication  → inicio de sesión y roles
        ├── Cloud Firestore          → barberías, servicios, citas, reseñas
        └── WorkManager (local)      → recordatorios en el dispositivo
```

Las reservas se confirman mediante **transacciones de Firestore**, que verifican la disponibilidad y registran la cita en una sola operación. El control de acceso por rol se aplica con las reglas de seguridad de Firestore, y los promedios de calificación se calculan solo a partir de reseñas válidas.
