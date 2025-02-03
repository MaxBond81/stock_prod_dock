FROM python:3.9

COPY ./requirements.txt ./requirements.txt 
RUN pip install -r ./requirements.txt

COPY . .

RUN python manage.py migrate

EXPOSE 5050

CMD ["gunicorn", "--bind", "0.0.0.0:5050", "stock_prod_dock.wsgi"]
