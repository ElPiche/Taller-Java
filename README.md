Proyecto creado para la materia Taller de sistemas de información JavaEE en UTEC.

Integrantes del proyecto:

Kevin Viera: kevin.viera@estudiantes.utec.edu.uy

Martin Antunez: martin.antunez@estudiantes.utec.edu.uy

Braian Granero: braian.granero@utec.edu.uy

Lucas Techera: fidel.techera@estudiantes.utec.edu.uy

Tecnologías utilizadas en el proyecto:

- Docker.
- Grafana.
- InfluxDB.
- MySQL.
- JMeter.
- JakartaEE


Estructura del proyecto.

El proyecto se encuentra estructurado por tres partes, infraestructura, sistema de tráfico y sistemas externos.

Infraestructura: Este sistema es el encargado de comunicarle al sistema de tráfico, los vehiculos que se encuentran circulando, en un caso real esto funcionaria con barreras, camaras, lectores de TAG, etc. 
En este caso se generará el paso de los vehiculos, apuntando a distintos endpoints del sistema de tráfico utilizando JMeter, emulando distintos casos de uso.

Sistema de tráfico: Este sistema se encuentra compuesto por 2 subsistemas, CORE es el encargado de gestionar la habilitación de vehiculos, la gestiín de pagos con sistemas externos y gestión de usuarios. Este subsistema se comunica con el subsistema de monitoreo,
el cual se encuentrá utilizando grafana para graficar, los recursos solicitados en la propuesta.

Sistemas externos: Este sistema se encuentra compuesto por 2 mock API las cuales simulan un pago con tarjeta de credito, o un pago con Sucive (Sistema de cobro de Uruguay).

Iteraciones.

-Iteración 1 capa de dominio: Esta etapa se centra en el desarrollo del sistema de tráfico, el mismo tiene una estructura que consta de 6 modulos, en los cuales se implementará logica de negocio, básica, sin persistencia por el momento.

-Iteración 2 integración sistemas externos: pendiente

-Iteración 3 Monitoreo:  pendiente

-Iteración 4 Messaging:  pendiente
