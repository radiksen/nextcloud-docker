# 🚀 Nextcloud Docker — ready to use

This repository allows you to quickly deploy **Nextcloud** with a **MariaDB** database using **Docker Compose**. Ideal for both local testing and server use.

---

## 🔧 Quick Start

```bash
git clone https://github.com/your-user/nextcloud-docker.git
cd nextcloud-docker
cp .env.example .env
docker compose up -d
```

Then open your browser: [http://localhost:8080](http://localhost:8080)

---

## 📦 What's included

- **Nextcloud 28** (Apache-based)
- **MariaDB 10.11** as the database
- Upload limit: **2 GB**
- Environment variables via `.env` file
- Data is persisted using named Docker volumes

---

## ⚙️ Configuration

All credentials and database config are stored in `.env` file.  
Use `.env.example` as a template:

```env
MYSQL_ROOT_PASSWORD=your-root-password
MYSQL_PASSWORD=your-nextcloud-password
MYSQL_DATABASE=nextcloud
MYSQL_USER=nextclouduser
```

---

## 🔐 Recommendations

- ⚠️ **Never commit your `.env` file** to the public repository!
- 🔒 For production use, configure **HTTPS** using a reverse proxy (e.g. Nginx, Traefik, or Caddy)
- 💾 Don't forget to back up your volumes regularly

---

## 🧩 Next steps

- Add SMTP and email setup for password recovery
- Enable external storage (e.g. S3, GDrive)
- Configure cron jobs for optimal performance
- Setup caching (Redis, APCu)

---

## 📄 License

MIT — free for personal and commercial use.
