# Self-Hosted Media Server - Docker Compose Configurations

This repository contains Docker Compose configurations for self-hosted media and automation applications. Each application has its own directory with a separate `docker-compose.yml` file for easy management.

## Applications Included

- **Plex** – Media server for streaming movies and TV shows.
- **Prowlarr** – Indexer manager for Sonarr and Radarr.
- **Radarr** – Movie management and automation.
- **Sonarr** – TV show management and automation.
- **Transmission** – Torrent client.
- **Watchtower** – Automated Docker container updates.

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/yashielsookdeo/apollo-sff-nas.git
```

### Navigate to the Desired App Folder

```bash
cd apollo-sff-nas/plex
```

### Deploy the Container Using Docker Compose

```bash
docker-compose up -d
```

Repeat for each service as needed.

## Environment Variables

Some services may require environment variables such as API keys, user credentials, or storage paths. These can be stored in a `.env` file (if supported by the app) or modified directly in `docker-compose.yml`.

## Updating Containers

Watchtower is configured to automatically update all running containers. If you need to update manually, run:

```bash
docker-compose pull && docker-compose up -d
```

## Contributing

If you have improvements or new configurations, feel free to submit a pull request.

## License

This project is open-source under the MIT License.