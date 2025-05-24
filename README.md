# Task Management APP (GraphQL + NestJS + React)
ここのcommitを取り消すrevert pull reqestに挑戦
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

## 感想
アプリ開発においてはただコードを書いて開発するのではなく、Dockerのようなアプリケーション実行環境を立ち上げる必要があったり、環境ごとの設定ファイルを使った構成管理など、実践的な開発には欠かせない知識が多くあることを今回のUdemyの講義から実感しました。
大変だったことは、エラーが出てきたとの対処にかなり時間がかかってしまったことです。chatGPTから提示されたコマンドを実行して状況がさらに複雑になってしまったことが何回かあるので、Webの情報も並行して確認して正確にエラー対応するべきだと思いました。
まだ全体的な復習が終えていないので、時間があるときにちゃんと復習してコードの理解に努めたいと思います。
