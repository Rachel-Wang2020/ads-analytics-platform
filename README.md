## Daily Progress Log

- Day 0（feb 4）: -Monorepo setup, workspace tooling, local infra bootstrapping
                -✅ 1) pnpm infra:up 能启动 Postgres + Redis
                -✅ 2) repo 有 apps/ packages/ infra/ 三层结构
                -✅ 3) pnpm dev / pnpm build / pnpm typecheck 有脚手架
                -✅ 4) @repo/types 能被未来的 apps 引用（paths 已就位）
- Day 1(feb 4):
              generator event -> raw_events -> aggregration job -> ads_metric_daily -> graphQL BFF -> react dashboard
  the dashboard never queries raw event tables directly, all analytical queries go through pre-aggregated rollup tables to guarantee predictable latency and cost

  Ownership
  data infra owns the schema(infra/db)
  worker owns event ingestion(apps/worker)
  aggregator owns rollup correctness(apps/worker another job)
  bff owns qurey contract + rbac + cache(apps/bff)
  fe owns interation + performance(apps/web)
  
  
  
- Day 2: 
- Day 3:
- Day 4:
- Day 5:
- Day 6:
- Day 7:
