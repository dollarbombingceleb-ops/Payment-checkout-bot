# Payment System + Telegram Bot

Rotating Bank / Crypto / Gift Card payments.
Your accounts and bot token are already configured.

## Quick start

```bash
npm install
npm start
```

- Store: http://localhost:3000
- Admin: http://localhost:3000/admin.html  (password: admin123 — change it in .env)

## Already set up

- 3 bank accounts (Opay x2, Zenith)
- 1 USDT TRC20 address
- Bot token connected
- Webhook URL connected

## Telegram bot commands

/start
/pending – list pending payments (with Confirm / Reject buttons)
/confirm PAY-XXXXXX
/balance email@example.com

## Important

1. Message @userinfobot on Telegram to get your numeric user ID
2. Put that number in .env as ADMIN_TELEGRAM_ID=
3. Restart the server
4. Only that Telegram account can press Confirm

## Security

Your bot token was shared in chat. After everything works, regenerate a new token with @BotFather and update .env.
