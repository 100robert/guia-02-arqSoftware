# Atributos de Calidad

## Mentelyx

| ID | Atributo de calidad | Escenario de calidad |
|---|---|---|
| AC01 | Rendimiento | Las operaciones frecuentes de aprendizaje, como obtener actividades, registrar respuestas, solicitar pistas y consultar retroalimentación, deben mantener tiempos de respuesta adecuados durante períodos de alta concurrencia. |
| AC02 | Escalabilidad | El sistema debe soportar aproximadamente 1 500 usuarios concurrentes durante una operación habitual y permitir escenarios de prueba con picos de hasta 15 000 usuarios concurrentes. |
| AC03 | Disponibilidad | Una falla parcial de un componente o instancia no debe provocar necesariamente la indisponibilidad completa de Mentelyx. |
| AC04 | Confiabilidad | Las respuestas e interacciones realizadas por los estudiantes no deben perderse ni registrarse accidentalmente más de una vez. |
| AC05 | Seguridad | La información personal, credenciales, progreso y resultados de los estudiantes deben estar protegidos frente a accesos no autorizados. |
| AC06 | Privacidad | La información individual relacionada con el aprendizaje de un estudiante solamente debe estar disponible para usuarios autorizados. |
| AC07 | Mantenibilidad | Los principales componentes del sistema deben estar organizados de manera que puedan modificarse sin afectar innecesariamente otras funcionalidades. |
| AC08 | Adaptabilidad | El sistema debe poder modificar las actividades presentadas en función de la evolución del perfil de aprendizaje del estudiante. |
| AC09 | Usabilidad | La interfaz debe permitir que un estudiante pueda realizar actividades, solicitar ayuda y consultar su progreso de manera sencilla desde dispositivos móviles o computadoras. |
| AC10 | Interoperabilidad | El sistema debe permitir futuras integraciones con otros servicios educativos mediante interfaces claramente definidas. |
| AC11 | Observabilidad | La solución debe permitir obtener información sobre errores, carga, tiempos de respuesta y comportamiento de sus principales componentes. |
| AC12 | Evolutividad | La incorporación de nuevas asignaturas o áreas de conocimiento no debe requerir rediseñar completamente la solución. |
| AC13 | Eficiencia de conectividad | Las funcionalidades principales de aprendizaje deben minimizar la transferencia innecesaria de datos y mantener una experiencia utilizable cuando el estudiante acceda mediante conexiones de capacidad limitada o inestable. |


## Escenario de Alta Concurrencia

Mentelyx está concebido como una plataforma que pueda ser utilizada por
estudiantes de diferentes instituciones educativas.

Durante determinadas situaciones, como evaluaciones diagnósticas, inicio de
programas académicos o actividades educativas de participación masiva, una
gran cantidad de estudiantes podría utilizar la plataforma simultáneamente.

Para efectos del análisis arquitectónico se establecen los siguientes
escenarios de carga:

- Operación habitual: aproximadamente 1 500 usuarios concurrentes.
- Incremento de demanda: entre 1 500 y 10 000 usuarios concurrentes.
- Escenario máximo de prueba: hasta 15 000 usuarios concurrentes.

La concurrencia no solamente implica estudiantes conectados, debido a que
cada sesión puede generar múltiples solicitudes relacionadas con actividades,
respuestas, contenidos, pistas, retroalimentación y progreso.

Por esta razón, rendimiento y escalabilidad constituyen atributos de calidad
relevantes para las futuras decisiones arquitectónicas.
