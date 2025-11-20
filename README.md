# EShop Microservices 

## Overview

A lightweight microservices based e‑commerce system built with **ASP.NET
Core**.\
It uses **Ocelot** as API Gateway, **RabbitMQ + MassTransit** for
messaging, **Redis** for the Basket service, **gRPC** for communication
between Discount and Basket, and multiple databases (**Postgres**,
**MongoDB**, **SQL Server**).\
All services run inside **Docker containers**.

## Services

-   **Catalog Service**
-   **Discount Service**
-   **Basket Service**
-   **Ordering Service**

## Technologies

-   ASP.NET Core
-   Ocelot API Gateway
-   RabbitMQ / MassTransit
-   Redis
-   gRPC
-   Docker
-   Postgres, MongoDB, SQL Server, Redis

## Run with Docker

``` bash
docker-compose up -d
```

## Notes

-   Use gRPC to get discount data inside Basket Service.
-   Use RabbitMQ for async communication between services.
-   Databases are isolated per service following microservice best
    practices.
