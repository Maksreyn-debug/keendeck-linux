# KeenDeck Linux

Консольный Linux для **Keenetic Omni KN-1410 / MT7628AN/NN**, 128 MiB RAM. Linux 6.6.110, BusyBox 1.36.1, MIPS32r2 little-endian, UART 57600 8N1.

**Experimental / source pre-release. Стабильной flash-прошивки пока нет.**

## Скачать исходники

[Релиз v1.0.0-rc1-source](https://github.com/Maksreyn-debug/keendeck-linux/releases/tag/v1.0.0-rc1-source)

Полный проект (107 файлов) находится в прикреплённом asset **KeenDeck-GitHub-v1.0.0-rc1-source.zip**. В нём README, сборочные скрипты, configs/DTS, rootfs, тесты, GitHub Actions workflow и отдельный read-only backup-профиль.

Скачивайте именно этот asset: автоматические GitHub Source code ZIP/TAR — снимок текущей ветки страницы проекта, полного дерева исходников в main пока нет.

SHA256 полного архива:
```text
c9331dceddc781722c54b9b4a2a3f2d4b00c85c3de3346004c2a71313c85847c
```

## Статус

- 26 локальных host unit-тестов и HTTP loopback передачи 32 MiB: PASS.
- Полная сборка очищенного публичного uImage и GitHub CI: NOT RUN.
- USB enumeration -62 остаётся нерешённой; Ethernet, повторные загрузки и часовая стабильность не квалифицированы.
- Flash install/default slot/fallback: NOT READY. Установщик не включён.
- Wi-Fi, разгон и входящий SSH-сервер отключены.
- Персональный SSH-ключ и дампы устройств исключены из архива.

## Начало работы

Распакуйте полный asset и прочитайте README.md, SAFE_BOOT.md и FLASH_INSTALL_STATUS.md. Основной образ предназначен сначала для RAM-тестирования через U-Boot/YMODEM; никакой автоматической записи во flash. Образы для ASUS несовместимы с KN-1410.

## Лицензии

В полном исходном архиве сохранены LICENSE и THIRD_PARTY_NOTICES.md. Проект содержит части с MIT/GPL и сторонние компоненты с собственными лицензиями; пользовательский ASCII сохраняет права автора.
