# Hola, soy Ángel Peñalver

**Desarrollador backend · Node.js · NestJS · TypeScript** — Remoto desde Venezuela (UTC-4)

Me especializo en que los datos queden bien aunque las cosas pasen a la vez o lleguen tarde: bloqueo de filas en PostgreSQL, webhooks idempotentes, trabajos en segundo plano con colas y búsqueda con Elasticsearch.

[![Portafolio](https://img.shields.io/badge/Portafolio-angel--dev.lat-2ea44f?style=flat)](https://angel-dev.lat)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-angelpenalver-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/angelpenalver)
[![Email](https://img.shields.io/badge/Email-contacto%40angel--dev.lat-D14836?style=flat&logo=gmail&logoColor=white)](mailto:contacto@angel-dev.lat)

---

## Proyectos

### [Atomic Ticket](https://github.com/AngelPenalver/atomic-ticket) — reservas con pagos
`NestJS` `PostgreSQL` `TypeORM` `Stripe` `Docker` `GitHub Actions`

- `SELECT … FOR UPDATE` para que dos reservas simultáneas no vendan el mismo asiento (el segundo recibe `409`).
- Webhooks de Stripe idempotentes: los duplicados y los eventos fuera de orden no cambian el resultado; un pago que llega tarde se reembolsa solo.
- Las reservas sin pagar caducan a los 15 minutos (cron) y liberan el asiento.
- 45 tests unitarios, migraciones de TypeORM y CI con GitHub Actions.

### [Product Search API](https://github.com/AngelPenalver/product-search-api) — prueba técnica en 3 días
`NestJS` `Elasticsearch` `PostgreSQL` `Docker`

- Búsqueda tolerante a errores de escritura, con filtros, orden, paginación y autocompletado.
- PostgreSQL como fuente de verdad; la indexación en Elasticsearch se hace mediante eventos.
- 33 tests unitarios. El README incluye lo que mejoraría hoy y por qué.

### [ContactShip AI Leads](https://github.com/AngelPenalver/contactship-ai-leads) — prueba técnica aprobada
`NestJS` `BullMQ` `Redis` `Gemini` `Docker`

- Crear un lead no espera a la IA: el endpoint encola el trabajo y un worker llama a Gemini.
- La respuesta se valida como JSON; si falla, se guarda un resultado por defecto.
- Sincronización automática por cron, deduplicación por email y caché con Redis.

---

## Stack

**Backend:** Node.js, NestJS, TypeScript, Express, REST, OpenAPI/Swagger
**Datos:** PostgreSQL, Redis, TypeORM, MySQL, MongoDB, Elasticsearch
**Integraciones:** Stripe y webhooks, BullMQ, Google Gemini, Auth0/OAuth2
**Calidad y DevOps:** Jest, Docker, GitHub Actions, Git, Linux
**También:** WordPress, WooCommerce y Elementor en producción (rendimiento PageSpeed de 29 a más de 90)

---

<sub>English: backend developer (Node.js · NestJS · TypeScript) focused on data consistency — row locking, idempotent webhooks, queues and search. Projects and demos at [angel-dev.lat/en](https://angel-dev.lat/en).</sub>
