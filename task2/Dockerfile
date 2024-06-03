FROM node:16-alpine

# создание директории приложения
WORKDIR /home/ilovedocker/app

# установка зависимостей
# астериск ("*") по возможности скопирует оба файла: package.json и package-lock.json
# тот же символ делает копирование опциональным, т. е. без файла сборка не упадёт
COPY hello.sh ./
# Флаг --omit=dev означает - "не ставить devDependencies"
# они не нужны нам в продакшен-окружении
# копируем исходный код
EXPOSE 3000
ENTRYPOINT ["sh hello.sh"]
