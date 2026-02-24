# Versiones por entornos (DEV / QA / PROD)

## Comandos Utilizados

### Odoo
    sudo docker exec -it odoo-dev odoo --version
    sudo docker exec -it odoo-qa odoo --version
    sudo docker exec -it odoo-prod odoo --version

### PostgresSQL
    sudo docker exec -it postgres-dev postgres --version
    sudo docker exec -it postgres-qa postgres --version
    sudo docker exec -it postgres-prod postgres --version
### Apache Hop
    Imagen detectada por 'Docker ps -a': 'apache/hop:2.17.0'

    sudo docker exec -it postgres-dev postgres --version
    sudo docker exec -it postgres-qa postgres --version
    sudo docker exec -it postgres-prod postgres --version

## Tabla de versiones
| Entorno | Odoo | PostgresSQL | Hop |
|---|---|---|
| DEV | Odoo Server 18.0-20251121 | postgres (PostgreSQL) 16.11 | apache/hop:2.17.0|
| QA | Odoo Server 18.0-20251121 | postgres (PostgreSQL) 16.11 | apache/hop:2.17.0|
| PROD | Odoo Server 18.0-20251121 | postgres (PostgreSQL) 16.11 | apache/hop:2.17.0|

## Observaciones
    Odoo y Postgres esta alineadas en los tres entorno (misma version)
    Hop tambien esta alineado por el tag de la imagen (`2.17.0`)
    