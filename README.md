## 👋 Welcome to psitransfer 🚀

Self-hosted psitransfer application

## 📋 Description

Self-hosted psitransfer application

## 🚀 Services

- **psitransfer**: psitransfer/psitransfer:latest

## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/psitransfer/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/psitransfer" ~/.local/srv/docker/psitransfer
cd ~/.local/srv/docker/psitransfer
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install psitransfer
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
SERVICE_USER=1000
SERVICE_GROUP=1000
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:3008

## 📂 Volumes

- `./rootfs/config/psitransfer` - Data storage
- `./rootfs/data/psitransfer` - Data storage

## 🔍 Logging

```shell
docker compose logs -f psitransfer
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
