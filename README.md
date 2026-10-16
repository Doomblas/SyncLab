# SyncLab

Simulador de sincronización y concurrencia desarrollado para la asignatura de Sistemas Distribuidos.

El proyecto implementa distintos problemas clásicos de concurrencia utilizando microservicios independientes desarrollados con Java y Spring Boot, acompañados de un frontend común para visualizar el comportamiento de los procesos en tiempo real.

## Objetivo

Demostrar el uso práctico de mecanismos de sincronización como:

- Semáforos contadores
- Exclusión mutua
- Productor - Consumidor
- Control concurrente de recursos compartidos
- Sincronización y orden de ejecución de procesos

## Módulos

### 01. Estacionamiento
Controla el acceso concurrente de 10 vehículos a un estacionamiento con capacidad máxima de 4 espacios mediante un semáforo contador.

### 02. Cajero automático
Protege el saldo compartido de una cuenta bancaria mediante exclusión mutua para evitar condiciones de carrera.

### 03. Productor - Consumidor
Simula una línea de producción con un buffer limitado y coordinación entre productores y consumidores.

### 04. Cruce de vehículos
Controla el acceso concurrente a un puente permitiendo únicamente una dirección de circulación activa a la vez.

### 05. Centro de impresión
Sincroniza las etapas de diseño, revisión e impresión respetando un orden obligatorio de ejecución.

## Arquitectura

El proyecto sigue una arquitectura basada en microservicios.

```text
SyncLab/
│
├── frontend/
│
├── estacionamiento-service/
├── cajero-service/
├── fabrica-service/
├── puente-service/
└── impresion-service/
