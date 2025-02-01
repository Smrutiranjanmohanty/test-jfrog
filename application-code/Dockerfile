FROM  ubuntu:22.04 

RUN  apt-get update && apt-get install -y python3-pip

WORKDIR /home/app

COPY application-code/requirement.txt .

RUN pip install -r requirement.txt

COPY . .

EXPOSE 5000

CMD [ "python3", "app.py" ]