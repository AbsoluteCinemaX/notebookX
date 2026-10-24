<div align="center">

# 📓 notebookX

**Единое рабочее пространство для заметок, документов и совместной работы**

*Вдохновлён Notion · Разрабатывается командой из трёх человек*

![Status](https://img.shields.io/badge/status-in%20development-orange)
![Go](https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)

</div>

---

## ✨ Возможности

- 🔐 Регистрация и аутентификация
- 🗂️ Рабочие пространства (Workspaces)
- 📝 Редактор страниц с форматированием текста
- 🌳 Вложенные страницы и иерархия контента
- 👥 Управление доступом и правами
- 📎 Загрузка файлов и изображений
- ⚡ Совместное редактирование в реальном времени
- 🔎 Поиск по контенту

> Список возможностей может меняться в процессе разработки.

## 🧰 Технологии

| Слой | Стек |
|---|---|
| **Backend** | Go, Gin, PostgreSQL, sqlc + pgx, golang-migrate, WebSocket |
| **Frontend** | React, TypeScript, Next.js, Tailwind CSS, Tiptap |
| **Infrastructure** | Docker Compose, GitHub Actions, Swagger/OpenAPI, MinIO, Redis |

## 🏗️ Архитектура

Модульный монолит:

```
Frontend (Next.js)  ──HTTP / WebSocket──▶  Backend (Go + Gin)
                                              │
                                  ┌───────────┴───────────┐
                              PostgreSQL                MinIO
                          (данные приложения)     (файлы и изображения)
```

## 👨‍💻 Команда

| Участник | Роль | Зона ответственности |
|---|---|---|
| **Абзал** | Backend | База данных PostgreSQL, миграции, sqlc/pgx, модели данных, оптимизация запросов |
| **Альмансур** | Backend | REST API на Gin, аутентификация и авторизация, права доступа, бизнес-логика, Swagger |
| **Исмаил** | Frontend | React/TypeScript UI, навигация и сайдбар, редактор Tiptap, интеграция с API |

## 🚀 Быстрый старт

**Требования:** Go, Node.js + npm, Docker + Docker Compose, Git

```bash
git clone https://github.com/YOUR_ORGANIZATION/notebookX.git
cd notebookX
cp .env.example .env   # настройте переменные окружения
```

> Инструкции по запуску backend, frontend и БД будут добавлены позже.

## 📌 Статус

🚧 **В разработке** — команда активно реализует основные функции и дополняет документацию.

## 📄 Лицензия

Будет определена перед первым публичным релизом.