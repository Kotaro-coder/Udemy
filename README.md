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

### Frontend
- **React** (v19.x)
- **Vite**
- **TypeScript**
- **Apollo Client**：GraphQL Client
- **MUI (Material UI)**：Material Design Support React UI flamework

### Backend
- **NestJS** (v10.x)
- **GraphQL (code-first)**：API Design

### API / Certification
- **Passport.js**：JWT Certification

### Database / ORM
- **PostgreSQL** (v15)：Relational Database Management System
- **Prisma** (v6)：DB Schema Management & Migration

### Infrastructure
- **Docker / Docker Compose**：For DB Startup