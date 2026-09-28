# Restricciones del Sistema

## Mentelyx

| ID | Restricción | Descripción |
|---|---|---|
| RC01 | Aplicación web | La primera versión deberá ser accesible mediante navegadores modernos. |
| RC02 | Mobile-first | La experiencia del estudiante deberá priorizar dispositivos móviles, manteniendo compatibilidad con tablets y computadoras. |
| RC03 | Infraestructura cloud | La solución deberá poder desplegarse utilizando infraestructura en la nube. |
| RC04 | Alta concurrencia | La solución deberá considerar aproximadamente 1 500 usuarios concurrentes en operación habitual y escenarios de prueba de hasta 15 000. |
| RC05 | Inteligencia artificial | Mentelyx deberá incorporar un componente inteligente para analizar el desempeño y contribuir a la personalización del aprendizaje. |
| RC06 | Bajo costo | Las decisiones tecnológicas deberán considerar el costo de infraestructura y permitir crecimiento progresivo. |
| RC07 | Privacidad | Los datos individuales de aprendizaje deberán ser accesibles únicamente por usuarios autorizados. |
| RC08 | Control de versiones | El código fuente y la documentación deberán gestionarse mediante Git y GitHub. |
| RC09 | Educación secundaria | La primera versión estará orientada inicialmente a estudiantes de educación secundaria. |
| RC10 | Dominio inicial | Matemática será el área curricular utilizada para validar la primera versión. |
| RC11 | Multiinstitución | La solución deberá permitir que diferentes instituciones educativas utilicen la misma plataforma manteniendo separada su información. |
| RC12 | Conectividad | La solución deberá considerar que algunos estudiantes pueden utilizar conexiones a Internet limitadas o inestables. |
| RC13 | Apoyo educativo | Mentelyx será una herramienta complementaria y no sustituirá la función pedagógica del docente. |

## Decisiones aún no establecidas

En esta etapa todavía no se consideran restricciones las siguientes
decisiones tecnológicas:

- estilo arquitectónico definitivo;
- lenguaje y framework de backend;
- tecnología de frontend;
- motor de base de datos;
- mecanismo de cache;
- sistema de mensajería;
- proveedor cloud;
- estrategia de balanceo;
- tecnología utilizada para desplegar el componente de inteligencia artificial.

Estas decisiones serán analizadas posteriormente tomando como base los
drivers arquitectónicos identificados.