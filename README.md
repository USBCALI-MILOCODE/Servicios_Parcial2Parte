# Parcial 2, parte 2.

Microservicios Common y Gateway.


## Ejercicios de teoria
### 1. Buscar y poner en esta parte el concepto de Spring Cloud Gateway

| Concepto             | Significado                                                                |
| ----------------- | ------------------------------------------------------------------ |
| Spring Cloud Gateway |Spring Cloud Gateway es un enrutador y servidor de paso de API construido sobre Spring Framework. Proporciona una manera flexible y potente de enrutar y filtrar las solicitudes HTTP que van hacia servicios internos o externos en una arquitectura de microservicios. |

### 2. Con la orientación del profesor colocar en este parte del documento el significado de cada una de las propiedades del anterior archivo

| Propiedades             | Significado                                                                |
| ----------------- | ------------------------------------------------------------------ |
| spring.cloud.gateway.mvc.routes[0].id: | Identificador único para la ruta del microservicio de usuarios.|
|spring.cloud.gateway.mvc.routes[0].uri: | URI donde se encuentra el microservicio de usuarios, usando un balanceador de carga. | 
| spring.cloud.gateway.mvc.routes[0].predicates: |  Especifica las condiciones que una solicitud debe cumplir para que sea dirigida a la ruta del microservicio de usuarios. En este caso, la condición es que la solicitud tenga la ruta /api/alumno/**. |
| spring.cloud.gateway.mvc.routes[0].filters | Filtro que elimina los dos primeros segmentos del URI de la solicitud antes de reenviarla al microservicio.|
