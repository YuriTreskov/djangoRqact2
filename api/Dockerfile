FROM python

RUN pip install --upgrade pip

COPY ./req.txt .
RUN pip install -r req.txt

COPY . /app
WORKDIR /app

COPY ./entrypoint.sh .
ENTRYPOINT ["sh","/app/entrypoint.sh"]