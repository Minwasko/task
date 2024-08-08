FROM python:3.12

WORKDIR /app

COPY requirements.txt /app/

RUN apt-get update && apt-get install -y g++

RUN pip install -r requirements.txt

COPY . /app

EXPOSE 5000

CMD ["flask", "run", "--host=0.0.0.0"]
