---
title: 'Module: site/app.py'
type: catalog
provenance: extracted
module: site/app.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `site.app`/
symbols:
  stripe_webhook: stripe_webhook().
  logger: logger.
  create_checkout_session: create_checkout_session().
  app: app.
  host: host.
  file_handler: file_handler.
  BACKEND_DATA_PATH: BACKEND_DATA_PATH.
  list_galaxies: list_galaxies().
  serve_museum_data: serve_museum_data().
  serve_data: serve_data().
  capture_enterprise_lead: capture_enterprise_lead().
  get_printify_session: get_printify_session().
  PRINTIFY_MAP: PRINTIFY_MAP.
  PRINTIFY_SHOP_ID: PRINTIFY_SHOP_ID.
  serve_index: serve_index().
  serve_assets: serve_assets().
  is_debug: is_debug.
  STRIPE_WEBHOOK_SECRET: STRIPE_WEBHOOK_SECRET.
  PRINTIFY_TOKEN: PRINTIFY_TOKEN.
---
# Module: [`site/app.py`](../../../../../raw/code/gitgalaxy/site/app.py)

## Functions
- `capture_enterprise_lead()` — [`L381`](../../../../../raw/code/gitgalaxy/site/app.py#L381) — documented in [site-app](../../concepts/site-app.md)
- `create_checkout_session()` — [`L137`](../../../../../raw/code/gitgalaxy/site/app.py#L137) — documented in [site-app](../../concepts/site-app.md)
- `get_printify_session()` — [`L74`](../../../../../raw/code/gitgalaxy/site/app.py#L74) — Creates an HTTP session that automatically retries failed Printify requests. — documented in [site-app](../../concepts/site-app.md)
- `list_galaxies()` — [`L97`](../../../../../raw/code/gitgalaxy/site/app.py#L97) — documented in [site-app](../../concepts/site-app.md)
- `serve_assets(path)` — [`L129`](../../../../../raw/code/gitgalaxy/site/app.py#L129) — documented in [site-app](../../concepts/site-app.md)
- `serve_data(path)` — [`L124`](../../../../../raw/code/gitgalaxy/site/app.py#L124) — documented in [site-app](../../concepts/site-app.md)
- `serve_index()` — [`L112`](../../../../../raw/code/gitgalaxy/site/app.py#L112) — documented in [site-app](../../concepts/site-app.md)
- `serve_museum_data(path)` — [`L118`](../../../../../raw/code/gitgalaxy/site/app.py#L118) — documented in [site-app](../../concepts/site-app.md)
- `stripe_webhook()` — [`L221`](../../../../../raw/code/gitgalaxy/site/app.py#L221) — documented in [site-app](../../concepts/site-app.md)

## Module values
- `BACKEND_DATA_PATH` — [`L67`](../../../../../raw/code/gitgalaxy/site/app.py#L67)
- `PRINTIFY_MAP` — [`L28`](../../../../../raw/code/gitgalaxy/site/app.py#L28) — documented in [site-app](../../concepts/site-app.md)
- `PRINTIFY_SHOP_ID` — [`L25`](../../../../../raw/code/gitgalaxy/site/app.py#L25) — documented in [site-app](../../concepts/site-app.md)
- `PRINTIFY_TOKEN` — [`L24`](../../../../../raw/code/gitgalaxy/site/app.py#L24) — documented in [site-app](../../concepts/site-app.md)
- `STRIPE_WEBHOOK_SECRET` — [`L23`](../../../../../raw/code/gitgalaxy/site/app.py#L23) — documented in [site-app](../../concepts/site-app.md)
- `app` — [`L50`](../../../../../raw/code/gitgalaxy/site/app.py#L50) — documented in [site-app](../../concepts/site-app.md)
- `file_handler` — [`L59`](../../../../../raw/code/gitgalaxy/site/app.py#L59) — documented in [site-app](../../concepts/site-app.md)
- `host` — [`L439`](../../../../../raw/code/gitgalaxy/site/app.py#L439) — documented in [site-app](../../concepts/site-app.md)
- `is_debug` — [`L438`](../../../../../raw/code/gitgalaxy/site/app.py#L438)
- `logger` — [`L56`](../../../../../raw/code/gitgalaxy/site/app.py#L56) — documented in [site-app](../../concepts/site-app.md)

