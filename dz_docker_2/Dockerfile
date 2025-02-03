FROM python:3.9

COPY ./requirements.txt ./requirements.txt 
RUN pip install -r ./requirements.txt

COPY . .

RUN python manage.py migrate

EXPOSE 8000

CMD ["gunicorn", "--bind", "0.0.0.0:8000", "stocks_ptoducts.wsgi"]
