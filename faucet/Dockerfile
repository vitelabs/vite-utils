FROM python:3.9.0-slim

WORKDIR /app

RUN pip3 install requests discord.py python-dotenv

COPY ./ /app

CMD [ "python3", "discord-bot.py" ]