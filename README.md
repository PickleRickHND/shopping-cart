# Carrito de Compras - Banco Cuscatlán Prueba Técnica

## Descripción
Esta es una solución basada en microservicios para un carrito de compras, desarrollada como parte de la prueba técnica para Banco Cuscatlán. La solución se implementa utilizando Spring Boot y sigue las directrices especificadas en la prueba.

## Requisitos
- VS Code
- JDK 11 o superior
- Maven o Gradle

## Arquitectura
La aplicación está compuesta por varios microservicios:
1. **Productos**: Actúa como un proxy hacia la API externa [Fake Store API](https://fakestoreapi.com) para obtener información de productos.
2. **Ordenes**: Gestiona las órdenes de compra.
3. **Pago**: Simula el proceso de pago.
4. **Clientes y Detalles de Ordenes**: Contiene las entidades y DTOs necesarios para implementar el mecanismo de pago (no se requieren servicios ni endpoints).
5. **Seguridad, Autenticación y Autorización (Opcional)**: Implementación opcional para obtener puntos adicionales, se evaluará solo si el resto de los puntos han sido implementados.

## Endpoints

### Productos
- **GET /productos**: Obtiene la lista de productos desde la API externa.

### Ordenes
- **POST /ordenes**: Crea una nueva orden.
- **GET /ordenes/{id}**: Obtiene los detalles de una orden específica.

### Pago
- **POST /pago**: Simula el proceso de pago para una orden.

### Seguridad (Opcional)
- **POST /auth/login**: Autentica un usuario y proporciona un token JWT.
- **POST /auth/register**: Registra un nuevo usuario.
