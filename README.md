# Robosoft Bot v10.3 Railway Ready

این ریپو برای اجرای ربات Robosoft روی Railway آماده شده است.

## فایل‌های مهم

- `Dockerfile`
- `railway.json`
- `.dockerignore`
- `railway.env.example`
- `RAILWAY_DEPLOY.md`
- `bot.py`
- `requirements.txt`

## شروع سریع روی Railway

1. در Railway گزینه `New Project` را بزن.
2. گزینه `Deploy from GitHub repo` را انتخاب کن.
3. این ریپو را انتخاب کن.
4. در بخش Variables حداقل این مقادیر را وارد کن:

```env
BOT_TOKEN=
ADMIN_IDS=
DATABASE_FILE=/data/robosoft_bot.sqlite3
```

5. یک Volume با مسیر `/data` بساز تا دیتابیس SQLite پاک نشود.
6. برای Callback درگاه‌ها دامنه Railway را داخل این مقدارها بگذار:

```env
PUBLIC_BASE_URL=https://YOUR-RAILWAY-DOMAIN.up.railway.app
IPN_CALLBACK_URL=https://YOUR-RAILWAY-DOMAIN.up.railway.app/nowpayments/ipn
```

راهنمای کامل داخل `RAILWAY_DEPLOY.md` است.
