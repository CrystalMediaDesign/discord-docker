FROM gorialis/discord.py:alpine-extras

WORKDIR /app

COPY requirements.txt ./
RUN pip install -r requirements.txt

COPY . .

CMD [ "python", "./bot.py" ]
