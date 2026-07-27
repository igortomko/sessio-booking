# sessio-booking

Собранная публичная страница онлайн-записи Sessio — https://booking.sessio.health

**Здесь только артефакт сборки.** Исходники живут в `igortomko/sessio` (каталог `booking/`,
экраны — `app/src/components/booking/*`). Правки вносить там; сюда попадает результат
`npm run build` (статический экспорт Next + `scripts/spa-fallback.mjs`).

`404.html` — копия `index.html`: токены ссылок живут в базе и ротируются, пререндерить
страницу под каждую невозможно, поэтому GitHub Pages отдаёт фолбэк на любой неизвестный
путь, а страница сама читает `location.pathname`.
