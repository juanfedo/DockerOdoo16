# DockerOdoo16
Odoo16 + Postgres

to fix "Database odoo_v16 not initialized, you can force it with `-i base`" error in another console write:

    docker-compose exec odoo_v16 bash

An after:

odoo -i base -d odoo_v16 --stop-after-init --db_host=postgres -r odoo -w odoo
