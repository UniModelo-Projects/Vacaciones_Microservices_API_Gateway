# API Gateway

El API Gateway es el punto de entrada único para todas las solicitudes de los clientes. Se encarga de enrutar el tráfico hacia los microservicios correspondientes basándose en la ruta de la URL.

## Detalles Técnicos
- **Puerto:** 8080
- **Tecnología:** Spring Cloud Gateway.
- **Enrutamiento:** Utiliza Eureka para localizar las instancias de los servicios.

## Rutas Configuradas
- `/productos/**` -> Redirige a `product-service`.
- `/ordenes/**` -> Redirige a `order-service`.
- `/pagos/**` -> Redirige a `payment-service`.

## Logs
Este servicio escribe logs en el log group `api-gateway-log-group` en CloudWatch (LocalStack).
