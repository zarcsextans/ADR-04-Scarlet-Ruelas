# ADR-05: Incorporación de una API REST en el sistema Biblioteca Digital

| Campo  | Valor |
| ------ | ----- |
| Autor  | Scarlet Angelina Ruelas |
| Fecha  | 12/06/2026 |
| Estado | Aceptado |

---
## Contexto

Se está desarrollando un sistema de Mi Biblioteca cuyo objetivo es gestionar libros, usuarios, préstamos, reservas y pagos de forma digital y organizada.

En versiones anteriores del proyecto, la aplicación estaba basada en MVC con persistencia local (JSON), lo que funcionaba para pruebas, pero generaba limitaciones importantes:

- Acoplamiento entre la interfaz y la lógica del sistema
- Dificultad para escalar o reutilizar el backend
- Limitaciones para futuras integraciones (por ejemplo, apps móviles o frontend separado)

Además, el proyecto debe alinearse con tecnologías vistas en clase como ASP.NET Core Web API y buenas prácticas de arquitectura moderna.

---
## Decisión

Se decidió incorporar una **API REST utilizando ASP.NET Core Web API** como capa de acceso principal a los datos del sistema Mi biblioteca.

Esta API expone los recursos principales del sistema mediante endpoints HTTP:

- Libros
- Usuarios
- Préstamos
- Reservas
- Pagos

También se integró Swagger para documentación y prueba de los endpoints.

---
## ¿Por qué?

Se eligió REST porque:

- Permite comunicación estándar entre cliente y servidor mediante HTTP
- Facilita el desacoplamiento entre frontend (MVC o futuras apps) y backend
- Es ampliamente utilizado en la industria del software
- Es compatible con ASP.NET Core y su ecosistema de Web API
- Permite escalar el sistema sin depender de una sola interfaz

---
