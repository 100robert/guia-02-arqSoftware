# Arquitectura inicial del sistema

## Diagrama de arquitectura

```mermaid
flowchart TD

%% =========================
%% ACTORES
%% =========================
subgraph ACTORES["ACTORES"]
    Estudiante["Estudiante"]
    Tutor["Tutor"]
    Bienestar["Bienestar Universitario"]
    Coordinador["Coordinador Académico"]
    Admin["Administrador"]
end

%% =========================
%% PRESENTACIÓN
%% =========================
subgraph PRESENTACION["PRESENTACIÓN"]
    Web["Aplicación Web"]
    API["API REST"]
end

%% =========================
%% LÓGICA DE NEGOCIO
%% =========================
subgraph NEGOCIO["LÓGICA DE NEGOCIO"]
    Auth["Autenticación y Roles"]
    Students["Estudiantes"]
    Academic["Información Académica"]
    Risk["Evaluación de Riesgo"]
    Alerts["Alertas"]
    Interventions["Intervenciones"]
    Tracking["Seguimiento"]
    Reports["Reportes"]
    Audit["Auditoría"]
end

%% =========================
%% DATOS
%% =========================
subgraph DATOS["DATOS"]
    BD["PostgreSQL"]
end

%% =========================
%% SISTEMAS EXTERNOS
%% =========================
subgraph EXTERNOS["SISTEMAS EXTERNOS"]
    AcademicSystem["Sistema Académico"]
    ML["Motor Inteligente / IA"]
    Notifications["Servicio de Notificaciones"]
end

%% =========================
%% FLUJO
%% =========================

ACTORES --> Web
Web --> API
API --> NEGOCIO
NEGOCIO --> BD

AcademicSystem --> Academic
Risk --> ML
Alerts --> Notifications
```

## Descripción

La arquitectura inicial se organiza en tres capas principales:

- **Presentación:** permite la interacción de estudiantes, tutores, responsables de bienestar, coordinadores y administradores mediante una aplicación web conectada a una API REST.

- **Lógica de negocio:** contiene los módulos responsables de autenticación, gestión de estudiantes, información académica, evaluación del riesgo, alertas, intervenciones, seguimiento, reportes y auditoría.

- **Datos:** almacena la información académica, evaluaciones de riesgo, intervenciones y demás información persistente utilizando PostgreSQL.

El sistema también contempla integración con un sistema académico como fuente de información, un motor inteligente encargado del análisis del riesgo y un servicio de notificaciones para la distribución de alertas.