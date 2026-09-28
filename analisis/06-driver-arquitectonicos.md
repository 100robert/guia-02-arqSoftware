# Drivers Arquitectónicos

## Mentelyx

Los drivers arquitectónicos representan aquellos requisitos, atributos de
calidad y restricciones que tendrán una influencia significativa sobre las
decisiones de arquitectura de Mentelyx.

| ID | Driver arquitectónico | Origen | ¿Por qué influye en la arquitectura? |
|---|---|---|---|
| DA01 | Mentelyx debe soportar aproximadamente 1 500 usuarios concurrentes durante la operación habitual y escenarios de prueba de hasta 15 000 usuarios concurrentes. | AC02, RC04 | Condicionará las estrategias de escalamiento, distribución de carga y despliegue. |
| DA02 | Las operaciones de aprendizaje deben mantener tiempos de respuesta adecuados durante períodos de alta concurrencia. | AC01 | Puede influir en procesamiento, almacenamiento, mecanismos de caché, distribución de contenido y comunicación entre componentes. |
| DA03 | Cada estudiante debe mantener un perfil individual de aprendizaje. | RF08, RF09 | Condicionará el almacenamiento y procesamiento del estado individual de una gran cantidad de estudiantes. |
| DA04 | El nivel de dominio debe actualizarse continuamente a partir de las interacciones realizadas por el estudiante. | RF23 | Condicionará la comunicación entre las actividades educativas, almacenamiento y componente inteligente. |
| DA05 | Mentelyx debe adaptar automáticamente las actividades y su dificultad según el desempeño del estudiante. | RF16-RF24, AC08 | Condicionará la organización del motor de personalización y su interacción con el perfil de aprendizaje. |
| DA06 | El sistema debe representar relaciones entre habilidades y conocimientos prerrequisitos. | RF21, RF22 | Influye en el modelo educativo utilizado para organizar contenidos y rutas de aprendizaje. |
| DA07 | Las respuestas, progreso y resultados del estudiante no deben perderse ni registrarse accidentalmente más de una vez. | AC04 | Condicionará las decisiones relacionadas con persistencia, consistencia y procesamiento confiable. |
| DA08 | Una falla parcial no debe provocar necesariamente la indisponibilidad completa de Mentelyx. | AC03 | Condicionará las estrategias de disponibilidad, aislamiento de fallos, redundancia y recuperación. |
| DA09 | La información educativa y personal debe ser accesible únicamente por usuarios autorizados. | AC05, AC06, RC07 | Condicionará autenticación, autorización, permisos y protección de datos. |
| DA10 | Mentelyx debe incorporar inteligencia artificial dentro del proceso de aprendizaje personalizado. | RC05 | Condicionará la separación de responsabilidades, procesamiento y comunicación entre el componente inteligente y el resto de la solución. |
| DA11 | La infraestructura debe mantener costos controlados incluso cuando existan grandes variaciones en la cantidad de usuarios. | AC12, RC06 | Condicionará las estrategias de despliegue, escalamiento y utilización de recursos cloud. |
| DA12 | Mentelyx debe permitir incorporar progresivamente nuevos niveles, áreas, temas y habilidades. | AC10, RC09 | Requiere evitar que la lógica del sistema quede fuertemente acoplada únicamente a Matemática de Secundaria. |
| DA13 | La experiencia del estudiante estará orientada principalmente a dispositivos móviles y deberá considerar conexiones limitadas. | RC02, RC15, AC13 | Puede influir en el tamaño de los recursos, mecanismos de caché, sincronización y diseño de las comunicaciones. |
| DA14 | Los simulacros y evaluaciones masivas pueden producir picos de solicitudes simultáneas. | RF73-RF77, AC02 | Condicionará el manejo de carga, procesamiento de respuestas, persistencia y generación de resultados. |
| DA15 | Mentelyx debe soportar distintos planes de acceso y controlar las funcionalidades disponibles para cada suscripción. | RF42-RF48, RC11 | Condicionará el modelo de autorización, estado de suscripciones y validación de acceso a funcionalidades. |
| DA16 | Los pagos de las suscripciones deberán procesarse mediante un servicio externo. | RF49, RC14 | Condicionará la integración con sistemas externos, manejo de errores, confirmaciones y consistencia del estado de una suscripción. |
| DA17 | Los convenios institucionales podrán modificar beneficios y precios sin cambiar la cuenta principal del estudiante. | RF50-RF56, RC12, RC16 | Condicionará la separación entre identidad del usuario, suscripción y beneficios institucionales. |
| DA18 | Ningún usuario podrá utilizar funcionalidades docentes sin haber sido previamente verificado. | RF57-RF63, RC13 | Condicionará el modelo de roles, estados de verificación, autorización y auditoría. |
| DA19 | Un docente únicamente podrá consultar información de estudiantes que tenga autorizados o asignados. | RF80-RF83, AC05, AC06 | Condicionará el control de acceso a información académica y las relaciones entre docentes y estudiantes. |
| DA20 | La plataforma debe permitir observar su comportamiento durante escenarios de alta carga. | AC11 | Condicionará la incorporación de métricas, registros, monitoreo y trazabilidad. |

## Drivers prioritarios

Los drivers con mayor impacto esperado sobre la futura arquitectura de
Mentelyx son:

**Escalabilidad y rendimiento**, debido a que la plataforma deberá atender una
cantidad elevada de usuarios y soportar escenarios de prueba de hasta
15 000 usuarios concurrentes.

**Aprendizaje personalizado**, debido a que cada estudiante mantiene un perfil
de conocimiento diferente y puede recibir contenidos, actividades y niveles
de dificultad distintos.

**Inteligencia artificial**, debido a que la estimación del dominio y la
adaptación del aprendizaje forman parte del núcleo funcional de Mentelyx.

**Confiabilidad**, debido a que las respuestas, evaluaciones y progreso son
utilizados posteriormente para modificar el perfil de aprendizaje del
estudiante.

**Simulacros y evaluaciones masivas**, debido a que pueden concentrar una
cantidad elevada de solicitudes en períodos cortos de tiempo.

**Seguridad y privacidad**, debido a que Mentelyx administrará cuentas,
información académica y diferentes niveles de autorización.

**Disponibilidad**, debido a que una falla parcial no debería producir la
interrupción completa de los principales servicios educativos.

**Costo**, debido a que la plataforma deberá aumentar su capacidad durante
picos de demanda sin mantener permanentemente infraestructura dimensionada
para el escenario máximo.

**Conectividad**, debido a que parte de los estudiantes puede acceder mediante
redes móviles o conexiones limitadas.

**Suscripciones e integración de pagos**, debido a que Mentelyx deberá mantener
coherencia entre pagos externos, estado de las suscripciones y funcionalidades
habilitadas.