Simple FHE-based anonymous elections app

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

переведи на китайский

## fhe_election_app
简单的基于 FHE（全同态加密）的匿名投票应用：Next.js 前端 + Hardhat 智能合约。

⸻

快速开始
	•	要求：Node.js 20 及以上
	•	安装依赖：
	•	前端：cd frontend && npm i
	•	合约：cd fhe_election_app_contracts && npm i

⸻

开发
	1.	启动本地区块链网络 / 编译合约

cd fhe_election_app_contracts
npm run compile

	2.	将部署数据（地址/ABI）导出到前端

npm run export:frontend

	3.	启动前端

cd ../fhe_election_app
npm run dev


⸻

部署到 Vercel
	•	Monorepo 结构： Next.js 应用位于 fhe_election_app/，智能合约位于 contracts/。
	•	Vercel 使用根目录下的 vercel.json：
	•	安装依赖：cd fhe_election_app && npm ci
	•	构建命令：cd fhe_election_app && npm run build
	•	在 Vercel 项目设置中，可以将 Root Directory 设置为 fhe_election_app（可选，因为 vercel.json 已定义）。

⸻

简单说明：
Next.js 应用位于 fhe_election_app/，智能合约在 contracts/。
Vercel 会读取根目录的 vercel.json 文件并执行：
	•	安装依赖：cd fhe_election_app && npm ci
	•	构建：cd fhe_election_app && npm run build
也可以在 Vercel 设置中将根目录指定为 fhe_election_app。
