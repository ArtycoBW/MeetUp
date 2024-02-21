Features:

- Обмен сообщениями в реальном времени с помощью Socket.io
- Отправка вложений в виде сообщений с помощью UploadThing
- Удаление и редактирование сообщений в режиме реального времени для всех пользователей
- Создавайте каналы для текстовых, аудио и видео звонков
- Разговоры 1:1 между пользователями
- Видеозвонки 1:1 между участниками
- Управление участниками (Kick, изменение роли гостя / модератора)
- Генерация уникальных пригласительных ссылок и полностью рабочая система приглашений
- Бесконечная загрузка сообщений партиями по 10 штук (tanstack/query)
- Создание и настройка сервера
- Красивый пользовательский интерфейс с использованием TailwindCSS и ShadcnUI
- Полная отзывчивость и мобильный пользовательский интерфейс
- Светлый / темный режим
- Websocket fallback: Опрос с оповещениями
- ORM с использованием Prisma
- База данных MySQL с использованием Planetscale
- Аутентификация с помощью Clerk

### Prerequisites

**Node version 18.x.x**

### Install packages

```shell
npm i
```

### Setup .env file


```js
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=
NEXT_PUBLIC_CLERK_SIGN_UP_URL=
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=


DATABASE_URL=

UPLOADTHING_SECRET=
UPLOADTHING_APP_ID=

LIVEKIT_API_KEY=
LIVEKIT_API_SECRET=
NEXT_PUBLIC_LIVEKIT_URL=
```

### Setup Prisma

Добавьте MySQL Database (Я использовал PlanetScale)

```shell
npx prisma generate
npx prisma db push

```

### Start the app

```shell
npm run dev
```

## Available commands

Running commands with npm `npm run [command]`

| command         | description                              |
| :-------------- | :--------------------------------------- |
| `dev`           | Starts a development instance of the app |
