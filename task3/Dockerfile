FROM node:16-alpine

# создание директории приложения
WORKDIR /home/ilovedocker/app

# копируем файлы для установки зависимостей
COPY package*.json ./

# установка зависимостей
RUN npm install --omit=dev

# копируем исходный код приложения
COPY src/ .

# открываем порт
EXPOSE 3032

# запускаем main.js
ENTRYPOINT ["node", "main.js"]
