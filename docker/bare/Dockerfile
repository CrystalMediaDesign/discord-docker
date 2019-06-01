FROM python:3-slim

WORKDIR /usr/src/app

COPY requirements.txt ./

RUN apt-get update

RUN pip install --no-cache-dir -r requirements.txt

RUN pip install --upgrade --force-reinstall --version websockets==4.0.1

COPY . .

CMD [ "python", "./bot.py" ]
