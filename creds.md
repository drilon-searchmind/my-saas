# --- 
# Guide

## - Link
https://www.freecodecamp.org/news/full-stack-saas-tanstack-start-elysia-neon/?ref=dailydev

# ---
# Neon:

## - Connect command
npx neonctl@latest init

## - Connection string
postgresql://neondb_owner:npg_h3kNlWxVA7pJ@ep-falling-shape-al78tb8y.c-3.eu-central-1.aws.neon.tech/neondb?sslmode=require

## - Commands
- Drizzle Studio / Database
```
bunx drizzle-kit studio
```

"It opens a small web UI (URL is printed in the terminal) connected using drizzle.config.ts — same DB as db:push (local 127.0.0.1:5432 / my_saas unless DATABASE_URL overrides).

You can add a script in package.json if you want:

"db:studio": "drizzle-kit studio""

- Postgres / psql:
```
docker exec -it my-saas-postgres psql -U postgres -d my_saas -c "\dt"
```