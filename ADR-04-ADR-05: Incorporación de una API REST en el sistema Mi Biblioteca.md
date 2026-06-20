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
