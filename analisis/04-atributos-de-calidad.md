# Atributos de Calidad

## Mentelyx

| ID | Atributo de calidad | Escenario de calidad |
|---|---|---|
| AC01 | Rendimiento | Las operaciones frecuentes de aprendizaje, como obtener actividades, registrar respuestas, solicitar pistas y consultar retroalimentación, deben mantener tiempos de respuesta adecuados incluso durante períodos de alta concurrencia. |
| AC02 | Escalabilidad | Mentelyx debe soportar aproximadamente 1 500 usuarios concurrentes durante una operación habitual y escenarios de prueba de hasta 15 000 usuarios concurrentes. |
| AC03 | Disponibilidad | Una falla parcial de un componente no debe provocar necesariamente la indisponibilidad completa de la plataforma. |
| AC04 | Confiabilidad | Las respuestas, resultados, progreso y operaciones asociadas a las suscripciones no deben perderse ni registrarse accidentalmente más de una vez. |
| AC05 | Seguridad | Las cuentas, información educativa, funcionalidades administrativas y operaciones de suscripción deben estar protegidas frente a accesos no autorizados. |
| AC06 | Privacidad | La información individual de aprendizaje únicamente debe estar disponible para el propio estudiante y los usuarios expresamente autorizados. |
| AC07 | Mantenibilidad | Los principales componentes del sistema deben organizarse de forma que los cambios en una funcionalidad no afecten innecesariamente a otras partes de Mentelyx. |
| AC08 | Adaptabilidad | La plataforma debe modificar las actividades y su dificultad en función de la evolución del perfil de aprendizaje del estudiante. |
| AC09 | Usabilidad | Las principales funcionalidades deben ser comprensibles y fáciles de utilizar para estudiantes desde dispositivos móviles y computadoras. |
| AC10 | Evolutividad | La incorporación de nuevos niveles, áreas, cursos y tipos de actividad no debe requerir reconstruir completamente la solución. |
| AC11 | Observabilidad | La plataforma debe permitir identificar errores, tiempos de respuesta, carga, utilización de recursos y comportamiento de los componentes principales. |
| AC12 | Eficiencia de costos | El uso de infraestructura y servicios de inteligencia artificial debe poder ajustarse a la demanda para evitar costos innecesarios durante períodos de baja utilización. |
| AC13 | Eficiencia de conectividad | Las funcionalidades principales deben minimizar transferencias innecesarias de datos y mantener una experiencia utilizable en conexiones limitadas o inestables. |
| AC14 | Integridad de pagos | Un cambio de plan o activación de una suscripción debe realizarse únicamente cuando el sistema pueda determinar correctamente el resultado de la operación de pago correspondiente. |

## Escenario de alta concurrencia

Mentelyx podrá ser utilizado directamente por estudiantes de diferentes
regiones y también por estudiantes beneficiados mediante convenios con
instituciones educativas.

Durante el uso cotidiano se plantea un escenario aproximado de 1 500 usuarios
concurrentes.

Determinadas actividades pueden producir incrementos importantes de demanda,
especialmente:

- evaluaciones programadas;
- simulacros masivos;
- inicio de nuevos ciclos educativos;
- publicación de nuevas actividades;
- períodos de preparación para exámenes.

Para las pruebas de arquitectura se considerará un escenario máximo de hasta
15 000 usuarios concurrentes.

Un usuario activo puede generar múltiples solicitudes relacionadas con
contenidos, ejercicios, respuestas, pistas, retroalimentación, progreso y
evaluaciones. Por esta razón, la cantidad de usuarios conectados no representa
por sí sola la totalidad de la carga que deberá soportar la plataforma.