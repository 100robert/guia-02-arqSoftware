# Restricciones del Sistema

## Mentelyx

| ID | Restricción | Descripción |
|---|---|---|
| RC01 | Aplicación web | La primera versión de Mentelyx deberá ser accesible mediante navegadores web modernos. |
| RC02 | Mobile-first | La experiencia del estudiante deberá priorizar dispositivos móviles, manteniendo compatibilidad con tablets y computadoras. |
| RC03 | Despliegue cloud | La solución deberá poder desplegarse utilizando infraestructura en la nube. |
| RC04 | Alta concurrencia | La arquitectura deberá considerar aproximadamente 1 500 usuarios concurrentes durante la operación habitual y escenarios de prueba de hasta 15 000 usuarios concurrentes. |
| RC05 | Inteligencia artificial | Mentelyx deberá incorporar un componente inteligente relacionado con el análisis del desempeño y la personalización del aprendizaje. |
| RC06 | Bajo costo | Las decisiones tecnológicas deberán considerar el costo de infraestructura y evitar mantener permanentemente recursos dimensionados para la carga máxima. |
| RC07 | Privacidad | La información individual de aprendizaje deberá estar disponible únicamente para usuarios autorizados. |
| RC08 | Control de versiones | El código fuente y la documentación del proyecto deberán gestionarse mediante Git y mantenerse en un repositorio compartido. |
| RC09 | Niveles educativos | Mentelyx se diseñará para permitir contenidos de Primaria, Secundaria y Preuniversitario. |
| RC10 | Alcance del prototipo | La primera versión funcional utilizará Matemática de nivel Secundaria como dominio de validación. |
| RC11 | Suscripciones | La solución deberá permitir diferentes niveles de acceso y contemplar planes de suscripción. |
| RC12 | Convenios opcionales | Mentelyx podrá establecer convenios con instituciones educativas, pero su funcionamiento no deberá depender de que exista un convenio. |
| RC13 | Verificación docente | Ningún usuario podrá obtener privilegios de docente sin completar previamente un proceso de aprobación definido por Mentelyx. |
| RC14 | Servicio externo de pagos | Las operaciones monetarias deberán procesarse mediante una pasarela de pago externa; Mentelyx no deberá almacenar directamente datos sensibles de tarjetas bancarias. |
| RC15 | Conectividad | La solución deberá considerar que determinados estudiantes pueden utilizar conexiones a Internet limitadas o inestables. |
| RC16 | Independencia institucional | Un estudiante deberá poder utilizar Mentelyx sin necesidad de estar vinculado a un colegio, academia o institución educativa asociada. |

## Decisiones tecnológicas aún no establecidas

En esta etapa todavía no se consideran restricciones las siguientes
decisiones:

- estilo arquitectónico definitivo;
- lenguaje del backend;
- framework de frontend;
- motor de base de datos;
- mecanismo de caché;
- tecnología de mensajería;
- proveedor cloud;
- estrategia de balanceo de carga;
- tecnología utilizada para implementar el componente de inteligencia
  artificial;
- proveedor de pagos;
- proveedor de notificaciones.

Estas decisiones deberán determinarse posteriormente tomando como base los
drivers arquitectónicos del sistema.