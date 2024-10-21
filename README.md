# 🚀 WorkStarter

> **💼 Простая утилита для автоматического запуска программ и открытия сайтов при старте твоего ПК**

<div align="center">

![GitHub stars](https://img.shields.io/github/stars/ivanoskov/workstarter?style=social)
![GitHub forks](https://img.shields.io/github/forks/ivanoskov/workstarter?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/ivanoskov/workstarter?style=social)
![GitHub last commit](https://img.shields.io/github/last-commit/ivanoskov/workstarter)

<img src="image.png" alt="preview" width="600"/>

</div>

## ✨ Возможности

- 🖥️ Автоматический запуск программ
- 🌐 Открытие веб-сайтов
- ⏱️ Настраиваемые задержки для каждой задачи
- 🎨 Графический интерфейс для управления задачами
- 🔧 Настройка через JSON-конфигурацию
- 📁 Хранение конфигурации в пользовательской директории
- 📝 Логирование во временную директорию

## 🛠️ Установка

1. Скачайте последнюю версию установщика WorkStarter с [страницы релизов](https://github.com/ivanoskov/workstarter/releases).
2. Запустите скачанный файл `workstarter_setup.exe`.
3. Следуйте инструкциям мастера установки.

После установки:
- Графический интерфейс WorkStarter будет доступен в меню "Пуск" Windows.
- Агент WorkStarter будет автоматически запускаться при старте системы.

## 🚀 Использование

1. Запустите "WorkStarter Configuration" из меню "Пуск" для настройки задач.
2. Добавьте нужные задачи через графический интерфейс.
3. WorkStarterAgent будет автоматически запускаться при старте системы и выполнять настроенные задачи.

## ⚙️ Конфигурация

WorkStarter хранит конфигурацию в файле `config.json` в пользовательской директории приложения. Вот пример структуры:

```json
{
  "tasks": [
    {
      "type": "open_link",
      "url": "https://www.example.com",
      "delay": 3
    },
    {
      "type": "open_program",
      "path": "C:\\Program Files\\Example\\example.exe",
      "delay": 5
    }
  ]
}
```

## 📊 Схема работы

```mermaid
graph TD
    A[Запуск WorkStarter] --> B{Чтение config.json}
    B --> C[Парсинг задач]
    C --> D[Создание асинхронных задач]
    D --> E{Выполнение задач}
    E --> F[Открытие ссылок]
    E --> G[Запуск программ]
    F --> H[Завершение работы]
    G --> H
```

## 🤝 Вклад в проект

Если хочешь внести свой вклад в WorkStarter, буду рад твоей помощи:

- 🐛 Сообщай о найденных ошибках
- 💡 Предлагай новые функции
- 🔧 Отправляй пулл-реквесты

## 📄 Лицензия

Этот проект распространяется под лицензией MIT - подробности в файле [LICENSE](LICENSE).

## 🙏 Благодарности

- [PyQt6](https://www.riverbankcomputing.com/software/pyqt/) за инструменты для создания GUI
- [asyncio](https://docs.python.org/3/library/asyncio.html) за асинхронные возможности

---

<div align="center">
  Создано с ❤️ by ivanoskov
</div>
