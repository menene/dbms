# 02 — PostgreSQL

Configuración para levantar una instancia de **PostgreSQL** junto con **Adminer** para visualizar y administrar los datos desde el navegador.

## Requisitos

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Levantar los contenedores

```bash
docker compose up -d
```

## Acceso

| Servicio | URL | Usuario | Contraseña |
|----------|-----|---------|------------|
| Adminer  | http://localhost:8080 | `postgres` | `root` |

En Adminer selecciona:
- **Sistema:** PostgreSQL
- **Servidor:** `postgres`
- **Usuario:** `postgres`
- **Contraseña:** `root`
- **Base de datos:** `dbms` (opcional)

## Detener los contenedores

```bash
docker compose down
```

Para eliminar también los volúmenes (borra los datos):

```bash
docker compose down -v
```
