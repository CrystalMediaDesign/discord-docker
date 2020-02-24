FROM gorialis/discord.py:extras

WORKDIR /app

RUN apk update && apk add chromium-chromedriver

COPY requirements.txt ./
RUN pip install -r requirements.txt

COPY . .

CMD [ "python", "./bot.py" ]
