## fhe_election_app

Простое приложение для анонимных выборов на основе FHE (Fully Homomorphic Encryption): фронтенд (Next.js) + смарт‑контракты (Hardhat).

### Быстрый старт
- Требования: Node.js 20+
- Установите зависимости:
- Frontend: `cd frontend && npm i`
- Contracts: `cd fhe_election_app_contracts && npm i`

### Разработка
1) Запуск локальной сети/компиляция
```
cd fhe_election_app_contracts
npm run compile
```

2) Экспорт данных для фронтенда (адреса/ABI)
```
npm run export:frontend
```

3) Запуск фронтенда
```
cd ../fhe_election_app
npm run dev
```

—

Simple FHE-based anonymous elections app: Next.js frontend + Hardhat smart contracts.

### Quick start
- Requirements: Node.js 20+
- Install deps:
- Frontend: `cd frontend && npm i`
- Contracts: `cd fhe_election_app_contracts && npm i`

### Development
1) Compile/contracts
```
cd fhe_election_app_contracts
npm run compile
```

2) Export deployment data to frontend (addresses/ABI)
```
npm run export:frontend
```

3) Run frontend
```
cd ../fhe_election_app
npm run dev
```

### Deploy на Vercel / Deploy to Vercel
- Monorepo layout: Next.js app в `fhe_election_app/`, контракты в `contracts/`.
- Vercel использует `vercel.json` в корне:
  - install: `cd fhe_election_app && npm ci`
  - build: `cd fhe_election_app && npm run build`
- В настройках проекта Vercel можно указать Root Directory = `fhe_election_app` (не обязательно, т.к. есть vercel.json).

- Next.js app lives in `fhe_election_app/` and contracts in `contracts/`.
- Vercel reads root `vercel.json`:
  - install: `cd fhe_election_app && npm ci`
  - build: `cd fhe_election_app && npm run build`
- Optionally set Vercel Root Directory to `fhe_election_app`.


