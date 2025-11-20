# EShop Microservices 

## Overview

A lightweight microservices-based e‑commerce system built with **ASP.NET
Core**.\
It uses **Ocelot** as API Gateway, **RabbitMQ + MassTransit** for
messaging, **Redis** for the Basket service, **gRPC** for communication
between Discount and Basket, and multiple databases (**Postgres**,
**MongoDB**, **SQL Server**).\
All services run inside **Docker containers**.

## Services

-   **API Gateway**: Ocelot
-   **Catalog Service**: MongoDB
-   **Discount Service**: Postgres + gRPC Server
-   **Basket Service**: Redis + gRPC Client
-   **Ordering Service**: SQL Server
-   **Event Bus**: RabbitMQ + MassTransit

## Technologies

-   ASP.NET Core Microservices
-   Ocelot API Gateway
-   RabbitMQ / MassTransit
-   Redis
-   gRPC
-   Docker / Docker Compose
-   Postgres, MongoDB, SQL Serve

## Run with Docker

``` bash
docker-compose up -d
```

## Notes

-   Use gRPC to get discount data inside Basket Service.
-   Use RabbitMQ for async communication between services.
-   Databases are isolated per service following microservice best
    practices.
