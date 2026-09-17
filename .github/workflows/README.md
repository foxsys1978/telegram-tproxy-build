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
