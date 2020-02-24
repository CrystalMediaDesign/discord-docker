FROM gorialis/discord.py:extras

WORKDIR /app

RUN apk update && apk add chromium-chromedriver chromium

COPY requirements.txt ./
RUN pip install -r requirements.txt

COPY . .

CMD [ "python", "./bot.py" ]
