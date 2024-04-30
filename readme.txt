Запись расходов по категориям
Запись доходов по категориям
Удаление расходов
Удаление доходов
Вывод текстовой статистики расходов за день/неделю/месяц/за все время
Вывод графической статистики расходов за день/неделю/месяц/за все время

#запуск из server.py
#нужно указать свой телеграм id (@username_to_id_bot) в middlewared.py либо закомментить две заглушки в server.py
бот в тг - @financiall_assistant_bot, меню в мобильной версии вызывается командой /start

Python
Pandas, matplotlib
SQLight3
aiogram
Docker


В Dockerfile заполнить переменные окружения

ENV BOT_API_TOKEN="" - Идентификатор бота

ENV MY_TELEGRAM_ID="" - Идентификатор пользователя

docker build -t tgfinances ./
docker run --name tg-finance-bot -v *YOUR LOCAL PATH*/db/:/home/db tgfinances