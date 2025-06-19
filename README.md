# Mihomo на роутерах Keenetic

Инструкция для запуска ядра **Mihomo** на роутерах **Keenetic**.

---

## ⚙️ Поддержка ядра

На данный момент поддержка Mihomo добавлена в **форк клиента xkeen**.  
Скоро она появится (или уже появилась) в официальной установке:

- [XKeen на GitHub](https://github.com/jameszeroX/XKeen)
- Рабочая бета версия xkeen с Mihomo от автора: [Инструкция в Telegram](https://t.me/c/2138190368/258/132588)

---

## 🧩 Пример конфигурации

В моём репозитории доступен пример конфигурации для Mihomo с маршрутизацией **Ru-Bundle от Легиза**:

- [config.yaml (raw)](https://raw.githubusercontent.com/OMchik33/Keenetic-Mihomo/refs/heads/main/config.yaml)
- Админ панель: [http://192.168.1.1:9090/ui](http://192.168.1.1:9090/ui)

---

## Установка конфига

Скачайте базовый конфигурационный файл:

```bash
curl -L -o /opt/etc/mihomo/config.yaml https://raw.githubusercontent.com/OMchik33/Keenetic-Mihomo/refs/heads/main/config.yaml
```

---

## 🖥 Подключение пользовательского интерфейса

Вы можете использовать различные пользовательские интерфейсы для управления Mihomo. Укажите один из URL в конфигурационном файле (`config.yaml`) в поле `external-ui-url`.

### Примеры:

- Интерфейс от MetaCubeX:

  ```yaml
  external-ui-url: "https://github.com/MetaCubeX/metacubexd/releases/latest/download/compressed-dist.tgz"
  ```

- Интерфейс Zashboard:

  ```yaml
  external-ui-url: "https://github.com/Zephyruso/zashboard/releases/latest/download/dist.zip"
  ```

---

## 🛠 Полезные инструменты

- [Документация по настройке Mihomo](https://wiki.metacubex.one/ru/config/)
- [Онлайн-конвертер подписок в YAML с маршрутизацией](https://dikozimpact.github.io/clash-convertor/)
- [Наборы правил маршрутизации от Legiz](https://github.com/legiz-ru/mihomo-rule-sets)
