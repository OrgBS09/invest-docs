# STRUCTURE — рабочая рутина

## Где запускать
Только пользователем `ubuntu`, из репозитория:
`/home/ubuntu/lab/invest/repos/invest-services`

## Что делает
- Генераторы из `tools/` формируют:
  - `doc/STRUCTURE-CLEAN.md` — фильтрованный срез кода/конфигов.
  - `doc/STRUCTURE-since-YYYY-MM-DD.md` — изменения с даты.
  - `doc/STRUCTURE-system-since-YYYY-MM-DD.md` — системные зоны.
  - `doc/INDEX-RAW-LINKS.md` — индекс RAW-ссылок для invest-docs.

## Как запустить вручную
```bash
sudo -iu ubuntu
cd /home/ubuntu/lab/invest/repos/invest-services
bash tools/gen_clean_structure.sh
bash tools/gen_structure_since.sh
bash tools/gen_system_structure.sh
bash tools/gen_index_raw_links.sh
git add doc/INDEX-RAW-LINKS.md doc/STRUCTURE-CLEAN.md doc/STRUCTURE-*.md
git commit -m "docs(structure): refresh"
git push origin lab

