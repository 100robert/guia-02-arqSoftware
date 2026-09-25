# Atributos de calidad

| ID | Atributo | Escenario de calidad |
|---|---|---|
| AC01 | Rendimiento | Las operaciones de consulta de estudiantes, alertas y dashboards deben mantener tiempos de respuesta adecuados durante períodos de alta demanda. |
| AC02 | Disponibilidad | El sistema debe continuar proporcionando las funcionalidades principales ante fallos parciales de una instancia de la aplicación. |
| AC03 | Escalabilidad | La arquitectura debe permitir soportar aproximadamente 1500 usuarios concurrentes en operación habitual y pruebas de carga de hasta 15000 usuarios concurrentes mediante escalamiento horizontal. |
| AC04 | Seguridad | La información académica y personal de los estudiantes debe estar protegida mediante autenticación, autorización basada en roles y mecanismos de protección de datos. |
| AC05 | Mantenibilidad | Los componentes del sistema deben organizarse de manera modular para permitir modificaciones sin afectar innecesariamente otros módulos. |
| AC06 | Auditabilidad | Las evaluaciones de riesgo, intervenciones y modificaciones relevantes deben mantener un registro que permita conocer cuándo y por quién fueron realizadas. |
| AC07 | Confiabilidad | Una falla durante el procesamiento de una evaluación de riesgo no debe provocar pérdida de información ni generar resultados duplicados. |