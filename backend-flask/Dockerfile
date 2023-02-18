FROM python:3.10-slim-buster

WORKDIR /backend-flask

COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt

COPY . .

ENV FLASK_ENV=development

COPY myscript.sh /backend-flask/myscript.sh
RUN chmod +x /backend-flak/myscript.sh

EXPOSE ${PORT}
CMD ["/backend-flask/myscript.sh"]
