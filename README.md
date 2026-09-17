# Telegram Android с WEB-прокси (tproxy)

Сборка Telegram Android с поддержкой WEB-прокси через tproxy-server.

## Как использовать GitHub Actions для сборки

1. **Создайте fork репозитория** в вашем GitHub аккаунте
2. **Добавьте workflow файл** в `.github/workflows/build.yml`
3. **Запустите сборку** через Actions → Build Patched Telegram Android → Run workflow
4. **Скачайте APK** из артефактов после завершения сборки

## Настройка прокси

После установки патченого Telegram:

1. Откройте Telegram → Настройки → Данные и диск → Прокси
2. Добавить прокси → **WEB**
3. Введите:
   - **Домен:** `foxsys.duckdns.org`
   - **Secret:** `d41608a28d3d2e91a169c8564ba17945`

Или используйте ссылку:
```
https://t.me/webproxy?server=foxsys.duckdns.org&secret=d41608a28d3d2e91a169c8564ba17945
```

## Требования

- Android 8.0+ (API 21+)
- Android System WebView 1.14.0+
- ~50 MB свободного места
- Доступ в интернет через HTTPS

## Особенности

- Работает через WebView (браузер внутри Telegram)
- Обходит блокировки через HTTPS трафик
- Требует патченый Telegram (не стандартный)
- Сервер: `foxsys.duckdns.org:443`

## Альтернативы

Если не хотите собирать Telegram:
1. Использовать **AmneziaVPN** с тем же сервером
2. Настроить **SOCKS5** прокси через локальное приложение
3. Использовать **MTProxy** в стандартном Telegram