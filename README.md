# home-media-stack

Application stack for easy home media server deployment with Docker Compose.

# Usage

1. Change `JELLYFIN_PublishedServerUrl` env variable in `docker-compose.yml` to your server's IP address.
2. Run `docker compose up -d`.
3. Add trusted domains in nextcloud: `docker exec --user www-data nextcloud php occ config:system:set trusted_domains 1 --value 10.8.0.4:8080`
