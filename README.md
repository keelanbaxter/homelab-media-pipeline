Homelab Media Pipeline

A secure and modular self-hosted media automation stack using Docker containers.

This project is configured for managing **legally acquired media only**.  
No piracy is encouraged or supported.

---

Stack Overview

| Service        | Description                                   |
|----------------|-----------------------------------------------|
| Jellyfin       | Media streaming server                        |
| Sonarr/Radarr  | TV and Movie organizer/renamer                |
| Prowlarr       | Indexer manager                               |
| qBittorrent    | Secure download client (via VPN tunnel)       |
| Jellyseerr     | Media request frontend                        |
| Home Assistant | Smart home automation                         |

---

Security Features

- UFW + Fail2Ban (external config)
- `.env` file excluded from Git
- User permission hardening

---

Usage

bash
git clone git@github.com:keelanbaxter/homelab-media-pipeline.git
cd homelab-media-pipeline
docker-compose up -d
