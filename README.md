# landing-static-nginx

Статический сайт (витрина) для демонстрации настройки домена + VPS + Nginx + HTTPS.

## Демо
https://antonk2.ru

## Что сделано
- Nginx раздаёт статику из `/var/www/antonk2.ru/public_html`
- HTTP → HTTPS редирект
- www → non-www редирект
- Защитные заголовки
- Сертификат Let’s Encrypt + автообновление

## Как задеплоить на Ubuntu (коротко)
1. Скопировать файлы в:
   `/var/www/antonk2.ru/public_html`
2. Прописать nginx server block для домена
3. Выпустить сертификат Let’s Encrypt
4. `sudo nginx -t && sudo systemctl reload nginx`
