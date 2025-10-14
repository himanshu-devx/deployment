# 🧭 Run Instructions

```bash
# 1. Clone project
git clone <your-repo-url>
cd <your-repo-name>


# 2. (Optional) Edit domains in Caddyfile
nano Caddyfile

# 3. Start all services
docker compose up -d

# 4. Check running containers
docker ps

# 5. Check logs
docker logs -f caddy
docker logs -f openobserve
docker logs -f fluent-bit

# 6. Access services
# Frontend: https://app.domain.com
# Backend:  https://api.domain.com
# Logs UI:  https://log.domain.com

# 7. Stop services
docker compose down

# 8. Remove all (including data)
docker compose down -v
