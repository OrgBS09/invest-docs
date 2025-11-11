# Итоги: Автопубликация docs и базовая инфраструктура

**Что сделано**
- GitHub Actions: из `invest-services/doc/` → в публичный `OrgBS09/invest-docs:main` (только с ветки `lab`).
- Добавлен sanity-check PAT, `fetch-depth: 0`, `subtree split` заменён на готовый action push-to-another-repository.
- Проверен триггер (paths: doc/**), публикация на GitHub Pages работает.

**Как пользоваться**
1) Редактируем/добавляем md в `doc/…` в ветке `lab`.  
2) `git add . && git commit -m "docs: ..." && git push origin lab` → через ~10–30 сек видим обновления в `invest-docs`.

**Секреты**
- `DOCS_PUSH_TOKEN` — fine-grained PAT, доступ к `OrgBS09/invest-docs`, permissions: Contents: Read & write.

**Хвосты/риски**
- При изменении названия ветки/репо — обновить workflow.
- Следить за сроком жизни PAT, вести ротацию.

