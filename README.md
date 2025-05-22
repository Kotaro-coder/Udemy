# Task Management APP (GraphQL + NestJS + React)

## Environment Setup

```bash
# get repository
git clone https://github.com/Kotaro-coder/Udemy.git
cd <repo>

# start infrastructure (Postgres)
docker compose up -d        # => localhost:5432

# backend setup and launch
cd backend
cp .env.example .env         # confirm DATABASE_URL
npm install
npx prisma migrate dev --name init   # first time only
npm run start:dev            # http://localhost:3000/graphql

# frontend setup and launch in another tab
cd ../frontend
npm install
npm run dev                  # http://localhost:5173
```

##  Technology Stacks

| Technology | Tools / Libraries |
| --- | --- |
| Frontend | React,Vite,Typescript, Apollo Client,MUI |
| Backend | NestJS,GraphQL(code-first) |
| API / Certification | Passport.js |
| Database / ORM | PostgreSQL Prisma |
| Infrastructure | Docker / Docker Compose | 
