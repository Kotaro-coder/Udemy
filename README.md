# Task Management APP (GraphQL + NestJS + React)

## Environment Setup

```bash
# get repository
git clone https://github.com/<user>/<repo>.git
cd <repo>

# start infrastructure (Postgres)
docker compose up -d        # => localhost:5432

# backend setup and launch
cd backend
cp .env.example .env         # confirm DATABASE_URL
npm install
npx prisma migrate dev --name init   # first time only
npm run start:dev            # http://localhost:3000/graphql

# frontend setup and launch（in another tab）
cd ../frontend
npm install
npm run dev                  # http://localhost:5173
```

##  Technology Stacks

### Frontend
- **React** (v19.x)
- **Vite**
- **TypeScript**
- **Apollo Client**：GraphQL クライアント（useQuery など）
- **MUI (Material UI)**：マテリアルデザイン対応 UI コンポーネント

### Backend
- **NestJS** (v10.x)
- **GraphQL (code-first)**：スキーマ駆動 API 設計

### API / 認証
- **Passport.js**：JWT 認証 / 認可ロジック（NestJS 統合）

### Database / ORM
- **PostgreSQL** (v15)：永続化用 DB
- **Prisma** (v6)：DB スキーマ管理 & マイグレーション

### Infrastructure
- **Docker / Docker Compose**：ローカル開発環境・DB 起動用