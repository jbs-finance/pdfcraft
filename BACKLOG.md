# BACKLOG

Это форк storytold/pdfcraft, собственной разработки в нём нет (все 840 коммитов пришли из upstream). Приоритеты продукта ведёт upstream, ниже ссылки на первоисточники, а не копия.

## Источники правды
- [docs/gaps.md](docs/gaps.md): ранжированный список недостатков относительно Acrobat Pro (рендеринг, редактирование существующего текста, Chinese UI, OCR, Office, Preflight и PDF/A/X/UA, подписи, теги доступности, производительность, RTL).
- [ROADMAP.md](ROADMAP.md), раздел «Upcoming»: очередь вех с оценками в часах.
- [docs/roadmap.md](docs/roadmap.md): таблица вех M0 .. M14.
- Open issues: `gh issue list -R storytold/pdfcraft`.

## Приоритеты (по ROADMAP.md, раздел Upcoming)
- P0: конвертация и обмен (Create PDF из Office, экспорт в Word с сохранением вёрстки, #773).
- P1: бэклог и платформа (сбои и неверные результаты, китайский UI, #826).
- P2: harness точности против Acrobat и решение по рендереру (M2, #841).
- P3: редактирование существующего контента (M7), OCR-языки и Office (M10), Preflight и PDF/A/X/UA (M11).
- P4: подписи для институций (M9), теги доступности (M12), полировка 1.0 (M14).

## Долги форка
- Не установлено: зачем форк создан в организации jbs-finance и планируется ли использовать его (сборка, доработки, синхронизация).
- Не настроена синхронизация с upstream: `git remote add upstream https://github.com/storytold/pdfcraft.git`, затем регулярный `git fetch upstream`. Порядок слияния: не установлено.
- Состояние CI в форке (`.github/workflows`: ci, freebsd, packaging-lint, release, windows-arm64): не проверено.
- В коде нет маркеров TODO и FIXME (поиск по `crates`, `xtask`, `apps`); долги ведутся в `docs/gaps.md`.
