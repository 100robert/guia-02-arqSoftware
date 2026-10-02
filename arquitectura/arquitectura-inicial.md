# Arquitectura inicial del sistema

## Marketplace de productos para mascotas

La arquitectura inicial del Marketplace se organiza utilizando una arquitectura en tres capas, separando las responsabilidades de presentación, lógica de negocio y acceso a datos.

Además, el sistema interactúa con diferentes actores y servicios externos necesarios para completar las operaciones del Marketplace.

## Diagrama de arquitectura

```mermaid
flowchart TD

    %% =========================
    %% ACTORES
    %% =========================
    subgraph ACTORES["ACTORES"]
        Cliente["Cliente"]
        Seller["Seller"]
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
        Usuarios["Usuarios"]
        Sellers["Sellers"]
        Catalogo["Catálogo"]
        Carrito["Carrito"]
        Pedidos["Pedidos"]
    end

    %% =========================
    %% DATOS
    %% =========================
    subgraph DATOS["DATOS"]
        BD["Base de datos"]
    end

    %% =========================
    %% SISTEMAS EXTERNOS
    %% =========================
    subgraph EXTERNOS["SISTEMAS EXTERNOS"]
        Pago["Pasarela de pago"]
        ERP["ERP"]
        Envio["Servicio de envío"]
    end

    %% =========================
    %% FLUJO PRINCIPAL
    %% =========================

    Cliente --> Web
    Seller --> Web
    Admin --> Web

    Web --> API
    API --> NEGOCIO

    Usuarios --> BD
    Sellers --> BD
    Catalogo --> BD
    Carrito --> BD
    Pedidos --> BD

    %% =========================
    %% INTEGRACIONES EXTERNAS
    %% =========================

    Pedidos --> Pago
    Pedidos --> Envio
    Catalogo --> ERP

    %% =========================
    %% DISTRIBUCIÓN HORIZONTAL
    %% =========================

    Cliente ~~~ Seller
    Seller ~~~ Admin

    Usuarios ~~~ Sellers
    Sellers ~~~ Catalogo
    Catalogo ~~~ Carrito
    Carrito ~~~ Pedidos

    Pago ~~~ ERP
    ERP ~~~ Envio