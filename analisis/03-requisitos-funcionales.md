# Requisitos Funcionales

## Mentelyx

Mentelyx es un centro educativo virtual orientado al aprendizaje personalizado
mediante inteligencia artificial. La plataforma permitirá el acceso directo
de estudiantes y podrá establecer convenios con instituciones educativas para
otorgar beneficios especiales a sus miembros.

## Gestión de usuarios y acceso

| ID | Requisito funcional |
|---|---|
| RF01 | El sistema debe permitir el registro de nuevos usuarios mediante una cuenta personal. |
| RF02 | El sistema debe permitir autenticar a los usuarios registrados. |
| RF03 | El sistema debe permitir recuperar el acceso a una cuenta cuando el usuario olvide sus credenciales. |
| RF04 | El sistema debe mantener diferentes roles de usuario de acuerdo con las funcionalidades que cada persona pueda utilizar. |
| RF05 | El sistema debe impedir que un usuario acceda a funcionalidades o información para las cuales no tenga autorización. |

## Perfil educativo del estudiante

| ID | Requisito funcional |
|---|---|
| RF06 | El sistema debe permitir al estudiante seleccionar su nivel educativo: Primaria, Secundaria o Preuniversitario. |
| RF07 | El sistema debe permitir registrar información académica básica necesaria para configurar la experiencia inicial del estudiante. |
| RF08 | El sistema debe mantener un perfil individual de aprendizaje para cada estudiante. |
| RF09 | El sistema debe registrar el historial de actividades y progreso del estudiante. |
| RF10 | El sistema debe permitir al estudiante cambiar de nivel educativo cuando corresponda, manteniendo su historial de aprendizaje. |

## Evaluación diagnóstica

| ID | Requisito funcional |
|---|---|
| RF11 | El sistema debe permitir al estudiante realizar una evaluación diagnóstica antes de iniciar una ruta de aprendizaje. |
| RF12 | El sistema debe registrar las respuestas proporcionadas durante la evaluación diagnóstica. |
| RF13 | El sistema debe analizar los resultados de la evaluación diagnóstica. |
| RF14 | El sistema debe identificar conocimientos dominados y conocimientos que requieren refuerzo. |
| RF15 | El sistema debe estimar un nivel inicial de dominio para las habilidades evaluadas. |

## Aprendizaje personalizado

| ID | Requisito funcional |
|---|---|
| RF16 | El sistema debe generar una ruta de aprendizaje personalizada a partir del perfil y nivel de dominio del estudiante. |
| RF17 | El sistema debe seleccionar contenidos y actividades de acuerdo con el nivel de conocimiento del estudiante. |
| RF18 | El sistema debe adaptar progresivamente la dificultad de las actividades según el desempeño del estudiante. |
| RF19 | El sistema debe aumentar la dificultad de las actividades cuando el estudiante demuestre dominio suficiente. |
| RF20 | El sistema debe proporcionar actividades de refuerzo cuando detecte dificultades persistentes. |
| RF21 | El sistema debe identificar conocimientos prerrequisitos necesarios cuando el estudiante presente dificultades en una habilidad. |
| RF22 | El sistema debe permitir retornar temporalmente a conocimientos prerrequisitos antes de continuar con contenidos más avanzados. |
| RF23 | El sistema debe actualizar el nivel de dominio después de las actividades realizadas por el estudiante. |
| RF24 | El sistema debe determinar cuándo un estudiante alcanza el nivel de dominio requerido para avanzar a una nueva habilidad o nivel. |

## Ejercicios y actividades

| ID | Requisito funcional |
|---|---|
| RF25 | El sistema debe presentar ejercicios relacionados con las habilidades que el estudiante se encuentra desarrollando. |
| RF26 | El sistema debe registrar las respuestas correctas e incorrectas realizadas durante los ejercicios. |
| RF27 | El sistema debe registrar la cantidad de intentos realizados en cada actividad. |
| RF28 | El sistema debe registrar el uso de pistas durante la resolución de ejercicios. |
| RF29 | El sistema debe proporcionar retroalimentación después de las respuestas del estudiante. |
| RF30 | El sistema debe permitir al estudiante solicitar pistas durante determinados ejercicios. |
| RF31 | El sistema debe evitar proporcionar directamente la respuesta cuando una pista tenga como objetivo orientar el proceso de resolución. |

## Contenidos educativos

| ID | Requisito funcional |
|---|---|
| RF32 | El sistema debe permitir al estudiante acceder a contenidos educativos correspondientes a su nivel. |
| RF33 | El sistema debe organizar los contenidos mediante niveles, áreas, temas y habilidades. |
| RF34 | El sistema debe permitir al estudiante buscar contenidos educativos disponibles en Mentelyx. |
| RF35 | El sistema debe recomendar contenidos relacionados con las dificultades detectadas durante el aprendizaje. |
| RF36 | El sistema debe permitir incorporar nuevas áreas educativas sin eliminar el historial previamente generado por los estudiantes. |

## Seguimiento del aprendizaje

| ID | Requisito funcional |
|---|---|
| RF37 | El sistema debe permitir al estudiante consultar su progreso general. |
| RF38 | El sistema debe permitir consultar el nivel de dominio alcanzado por área, tema y habilidad. |
| RF39 | El sistema debe mostrar las habilidades que el estudiante ha dominado y aquellas que todavía requieren refuerzo. |
| RF40 | El sistema debe permitir al estudiante continuar su proceso de aprendizaje desde el punto donde lo dejó. |
| RF41 | El sistema debe mantener un historial de la evolución del nivel de dominio del estudiante. |

## Planes y suscripciones

| ID | Requisito funcional |
|---|---|
| RF42 | El sistema debe permitir ofrecer diferentes planes de acceso a Mentelyx. |
| RF43 | El sistema debe permitir disponer de un nivel de acceso gratuito con funcionalidades limitadas. |
| RF44 | El sistema debe permitir disponer de planes de pago con funcionalidades adicionales. |
| RF45 | El sistema debe mostrar al usuario las funcionalidades disponibles según su plan vigente. |
| RF46 | El sistema debe permitir al usuario contratar o cambiar un plan de suscripción. |
| RF47 | El sistema debe registrar el estado y vigencia de la suscripción de un usuario. |
| RF48 | El sistema debe restringir las funcionalidades exclusivas de los planes de pago cuando el usuario no posea una suscripción válida. |
| RF49 | El sistema debe integrarse con un servicio de pago para procesar las suscripciones cuando se implemente el módulo comercial. |

## Convenios con instituciones educativas

| ID | Requisito funcional |
|---|---|
| RF50 | El sistema debe permitir registrar instituciones educativas que mantengan un convenio vigente con Mentelyx. |
| RF51 | El sistema debe permitir definir beneficios asociados a cada convenio institucional. |
| RF52 | El sistema debe permitir verificar que un usuario pertenece a una institución educativa con convenio antes de otorgarle beneficios institucionales. |
| RF53 | El sistema debe permitir que un estudiante perteneciente a una institución aliada acceda a funcionalidades gratuitas definidas por el convenio. |
| RF54 | El sistema debe permitir aplicar descuentos en determinados planes de suscripción a usuarios pertenecientes a instituciones aliadas. |
| RF55 | El sistema debe registrar la institución con la que se encuentra vinculado un usuario cuando utilice un beneficio de convenio. |
| RF56 | El sistema debe retirar los beneficios institucionales cuando el convenio o la condición de acceso correspondiente deje de estar vigente. |

## Docentes

| ID | Requisito funcional |
|---|---|
| RF57 | El sistema debe permitir que una persona solicite incorporarse a Mentelyx como docente. |
| RF58 | El sistema debe solicitar información que permita evaluar una solicitud de incorporación como docente. |
| RF59 | El sistema debe mantener las solicitudes de docentes en estado pendiente hasta que sean revisadas. |
| RF60 | El sistema debe permitir a un operador autorizado de Mentelyx aprobar o rechazar solicitudes de docentes. |
| RF61 | El sistema debe otorgar funcionalidades de docente únicamente después de que la solicitud correspondiente haya sido aprobada. |
| RF62 | El sistema debe permitir registrar las áreas o especialidades educativas asociadas a un docente. |
| RF63 | El sistema debe permitir desactivar los privilegios de docente cuando corresponda. |

## Administración de Mentelyx

| ID | Requisito funcional |
|---|---|
| RF64 | El sistema debe permitir a los operadores autorizados administrar los niveles educativos disponibles. |
| RF65 | El sistema debe permitir administrar áreas, temas y habilidades educativas. |
| RF66 | El sistema debe permitir definir relaciones de prerrequisito entre habilidades. |
| RF67 | El sistema debe permitir administrar los contenidos educativos disponibles. |
| RF68 | El sistema debe permitir administrar ejercicios y clasificarlos según nivel, área, tema, habilidad y dificultad. |
| RF69 | El sistema debe permitir administrar los planes de suscripción ofrecidos por Mentelyx. |
| RF70 | El sistema debe permitir administrar convenios y beneficios institucionales. |
| RF71 | El sistema debe permitir consultar y gestionar cuentas de usuario cuando sea necesario. |
| RF72 | El sistema debe registrar las operaciones administrativas relevantes realizadas dentro de la plataforma. |

## Simulacros y evaluaciones

| ID | Requisito funcional |
|---|---|
| RF73 | El sistema debe permitir ofrecer evaluaciones o simulacros a los estudiantes. |
| RF74 | El sistema debe registrar las respuestas realizadas durante un simulacro. |
| RF75 | El sistema debe calcular los resultados obtenidos por el estudiante al finalizar una evaluación o simulacro. |
| RF76 | El sistema debe analizar los resultados obtenidos para identificar fortalezas y dificultades. |
| RF77 | El sistema debe utilizar los resultados de las evaluaciones, cuando corresponda, para actualizar el perfil de aprendizaje del estudiante. |

## Notificaciones

| ID | Requisito funcional |
|---|---|
| RF78 | El sistema debe generar notificaciones relacionadas con actividades, progreso, suscripciones o evaluaciones cuando corresponda. |
| RF79 | El sistema debe permitir al usuario consultar sus notificaciones dentro de la plataforma. |
## Acompañamiento docente

| ID | Requisito funcional |
|---|---|
| RF80 | El sistema debe permitir asociar estudiantes con docentes verificados cuando el servicio educativo contratado contemple acompañamiento docente. |
| RF81 | El sistema debe permitir al docente consultar únicamente el progreso de los estudiantes que tenga asignados. |
| RF82 | El sistema debe permitir al docente registrar orientaciones o retroalimentaciones dirigidas a los estudiantes que tenga asignados. |
| RF83 | El sistema debe impedir que un docente consulte información académica de estudiantes que no se encuentren bajo su autorización. |