# Weazel News — Article Kit V3 (Ultra Simple)

## Что это
Мини‑сайт для быстрого создания статьи и отправки её в Discord канал Weazel News (кураторам или сразу в общий). Без БД, без сложной логики.

## Быстрый старт (Vercel)
1) Создай 1–2 вебхука в Discord:
   - DISCORD_WEBHOOK_PUBLIC — публичный канал Weazel News
   - DISCORD_WEBHOOK_CURATORS — закрытый канал кураторов (опционально)
2) Залей папку в GitHub → **Import** в Vercel.
3) В Vercel → Settings → Environment Variables:
   - `DISCORD_WEBHOOK_PUBLIC` = URL из шага 1
   - `DISCORD_WEBHOOK_CURATORS` = URL (можно пустым — тогда всё уйдёт в public)
4) Deploy.
5) Открой сайт, заполни форму, выбери галочку «Отправить кураторам» или выключи её для публичной публикации → **Отправить**.

## Локально
```bash
npm i
npm run dev
# открой http://localhost:5173
```

## Замечания
- Обложка попадает в embed Discord. Галерея уходит дополнительными файлами.
- Поле «Подписанты» — просто текстовый блок. Каждый с новой строки: `Имя — Роль`.
- Если нужна модерация/архив — переходи к версии V2 с Supabase.
