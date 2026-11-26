# Nillacup Sales (فروش سرد نیلاکاپ)

مخزن خصوصی برای راه‌اندازی تیم فروش سرد نیلاکاپ.

## ساختار
- `meetings/` یادداشت و پاسخ هر جلسه (یک پوشه برای هر جلسه، با تاریخ میلادی)
- `docs/` ICP، ساختار CRM، اسکریپت‌ها، برنامهٔ آموزش، آگهی استخدام
- `questions-form.html` فرم سؤال‌ها (با دابل‌کلیک در مرورگر باز می‌شود؛ پاسخ‌ها فقط در همان مرورگر ذخیره می‌شود. خروجی Markdown را در `answers.md` جلسه بچسبانید)

## تصمیم‌ها
ثبت تصمیم‌های نهایی هر جلسه در `meetings/<تاریخ>/notes.md`.

## تنظیمات Claude Code
- `CLAUDE.md`: قواعد و زمینهٔ پروژه
- `.claude/skills/meeting-notes`: دستور `/meeting-notes` برای ثبت جلسه
- `.claude/skills/project-conventions`: قواعد نوشتن (خودکار)
- `.claude/agents/sales-ops-reviewer.md`: بازبین همخوانی `docs/` با تصمیم‌ها
- `.claude/settings.json` و `.claude/hooks/`: تأیید قبل از `git push` و قفل صورت‌جلسه‌های گذشته
