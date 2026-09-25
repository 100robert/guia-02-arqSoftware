# Drivers arquitectónicos

| ID | Driver arquitectónico | Origen | ¿Por qué influye en la arquitectura? |
|---|---|---|---|
| DA01 | El sistema debe soportar aproximadamente 1500 usuarios concurrentes y picos de prueba de hasta 15000 usuarios. | AC03 - Escalabilidad | Obliga a considerar escalamiento horizontal, balanceo de carga y reducción de estado dentro de las instancias. |
| DA02 | Las consultas de alertas, estudiantes y dashboards deben mantener tiempos de respuesta adecuados durante alta concurrencia. | AC01 - Rendimiento | Influye en el uso de caché, optimización de consultas y procesamiento asíncrono. |
| DA03 | La información académica y de riesgo debe estar protegida. | AC04 - Seguridad | Obliga a implementar autenticación, autorización por roles y protección de datos sensibles. |
| DA04 | El procesamiento masivo de evaluaciones de riesgo no debe bloquear la aplicación. | RF05, AC07 | Influye en la utilización de colas y procesamiento asíncrono mediante workers. |
| DA05 | El motor inteligente debe poder evolucionar independientemente de la aplicación principal. | RC06 | Justifica separar el servicio de evaluación inteligente del backend principal. |
| DA06 | El sistema debe seguir disponible ante la falla de una instancia del backend. | AC02 - Disponibilidad | Influye en el despliegue de múltiples instancias detrás de un balanceador de carga. |
| DA07 | Las operaciones relevantes deben mantener trazabilidad. | AC06 - Auditabilidad | Requiere registro de auditoría de evaluaciones, intervenciones y modificaciones. |
| DA08 | La solución debe tener bajo costo de operación. | RC10 | Favorece tecnologías open source, contenedores y escalamiento según demanda. |