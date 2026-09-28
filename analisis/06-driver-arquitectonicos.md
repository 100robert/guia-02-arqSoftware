# Drivers Arquitectónicos

## Mentelyx

Los drivers arquitectónicos representan aquellos requisitos, atributos de
calidad y restricciones que tendrán una influencia significativa en las
decisiones de arquitectura de Mentelyx.

| ID | Driver arquitectónico | Origen | ¿Por qué influye en la arquitectura? |
|---|---|---|---|
| DA01 | El sistema debe soportar aproximadamente 1 500 usuarios concurrentes en operación habitual y escenarios de prueba de hasta 15 000 usuarios concurrentes. | AC02, RC04 | Condicionará las estrategias de escalamiento, distribución de carga y despliegue. |
| DA02 | Las operaciones de aprendizaje deben mantener tiempos de respuesta adecuados durante períodos de alta concurrencia. | AC01 | Puede influir en almacenamiento, procesamiento, mecanismos de caché, distribución de contenidos y comunicación entre componentes. |
| DA03 | Cada estudiante debe mantener un perfil individual de aprendizaje. | RF05 | Condicionará la forma de almacenar y administrar el estado de miles de estudiantes simultáneamente. |
| DA04 | El nivel de dominio debe actualizarse a partir de las interacciones del estudiante. | RF08, RF09, RF10 | Puede requerir separar las responsabilidades de procesamiento y modelado del aprendizaje. |
| DA05 | La plataforma debe generar rutas y actividades diferentes según el perfil de cada estudiante. | RF11, RF12, AC08 | Condicionará la organización del componente responsable de la personalización. |
| DA06 | El sistema debe identificar relaciones entre habilidades y conocimientos prerrequisitos. | RF19, RF20, RF28 | Influye en la representación y organización del conocimiento educativo. |
| DA07 | Las respuestas de los estudiantes no deben perderse ni registrarse accidentalmente más de una vez. | AC04 | Condicionará las decisiones relacionadas con persistencia, consistencia y procesamiento confiable. |
| DA08 | Mentelyx debe continuar prestando sus principales funcionalidades frente a fallos parciales. | AC03 | Condicionará las estrategias de disponibilidad, redundancia y recuperación. |
| DA09 | La información de una institución, grupo o estudiante solo debe poder ser consultada por usuarios autorizados dentro de su ámbito correspondiente. | AC05, AC06, RC07, RF34 | Condicionará la autenticación, autorización, aislamiento de información y diseño del modelo de permisos. |
| DA10 | La solución debe incorporar inteligencia artificial para modelar el aprendizaje del estudiante. | RC05 | Condicionará la separación de responsabilidades y la integración entre el componente inteligente y el resto de la plataforma. |
| DA11 | La solución debe mantener un costo de infraestructura controlado. | RC06 | Condicionará las estrategias de despliegue, escalamiento y utilización de recursos cloud. |
| DA12 | La experiencia estará orientada principalmente a dispositivos móviles. | RC02 | Condicionará la entrega de contenidos, tamaño de recursos, rendimiento del frontend y comunicaciones con los servicios del sistema. |
| DA13 | Mentelyx debe poder incorporar nuevas asignaturas en el futuro. | AC12, RC10 | Requiere evitar que la lógica del sistema quede fuertemente acoplada únicamente a Matemática. |
| DA14 | La plataforma debe permitir supervisar su comportamiento durante escenarios de alta carga. | AC11 | Condicionará posteriormente la incorporación de métricas, logs, monitoreo y trazabilidad. |
| DA15 | Diferentes instituciones educativas deben utilizar la misma plataforma manteniendo su información correctamente aislada. | RC11, RF30, RF34 | Condicionará la organización de usuarios, permisos, datos e identificación de la institución a la que pertenece cada recurso. |
| DA16 | Los estudiantes pueden acceder mediante conexiones de Internet limitadas o inestables. | RC12, AC13 | Puede influir en el tamaño de recursos, estrategias de caché, sincronización, manejo de fallos de red y diseño de la aplicación cliente. |

## Drivers prioritarios

Los drivers con mayor impacto esperado sobre la futura arquitectura son:

**Escalabilidad y rendimiento**, debido a los escenarios de hasta 15 000
usuarios concurrentes.

**Personalización del aprendizaje**, debido a que cada estudiante mantiene
un estado de conocimiento diferente y puede recibir actividades distintas.

**Inteligencia artificial**, debido a que la estimación del dominio y el
análisis del desempeño forman parte del núcleo funcional de Mentelyx.

**Confiabilidad**, debido a que las respuestas de los estudiantes representan
información fundamental para actualizar correctamente sus perfiles de
aprendizaje.

**Disponibilidad**, debido a que una falla parcial no debería producir la
interrupción completa de la plataforma.

**Seguridad y aislamiento de datos**, debido a que Mentelyx será utilizado por
diferentes instituciones educativas y cada usuario deberá acceder únicamente
a la información que le corresponda.

**Conectividad**, debido a que algunos estudiantes podrían acceder desde
conexiones limitadas o inestables.

**Costo**, debido a que la solución debe poder aumentar su capacidad durante
picos de carga sin mantener permanentemente infraestructura dimensionada
para el escenario máximo.