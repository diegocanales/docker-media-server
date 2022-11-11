# Docker Media Server

## URLs

- Homepage: http://127.0.0.1
- Jellyfin: http://127.0.0.1:8096/
- Sonarr: http://127.0.0.1:8989/
- Radarr: http://127.0.0.1:7878/
- Bazarr: http://127.0.0.1:6767/
- Jacket: http://127.0.0.1:9117/
- qBittorrent: http://127.0.0.1:8080/
- FileBrowser: http://127.0.0.1:8085/

## Project Structure

```text
.
├── docker-compose.yaml
├── downloads/
├── media
│   ├── movies
│   └── series
├── README.md
└── services
    ├── bazarr
    ├── filebrowser
    ├── homepage
    ├── jackett
    ├── jellyfin
    ├── qbittorrent
    ├── radarr
    └── sonarr
```

## Environment file template

```text
MY_PUID=1000
MY_PGID=1000
TZ=America/Santiago

DOWNLOADS_DIR=./downloads
MEDIA_DIR=./media
TV_DIR=${MEDIA_DIR}/series
MOVIES_DIR=${MEDIA_DIR}/movies
```
