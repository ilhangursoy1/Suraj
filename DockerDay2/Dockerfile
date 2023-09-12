FROM python:3.9-slim-buster

# Set the working directory to /app
WORKDIR /app

COPY requirements.txt requirements.txt 

COPY . .

RUN pip3 install -r requirements.txt
RUN apt-get update
#apt-get install -y vim
EXPOSE 5000

# CMD ["python3", "-m","flask","run", "--host=0.0.0.0"]
CMD ["python3", "app.py"]