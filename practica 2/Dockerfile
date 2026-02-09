FROM python:3.12-alpine3.17

WORKDIR /app

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

COPY . .

#permite cambios en el codigo sin necesidad de reconstruir la imagen.
CMD [ "python", "-m", "flask", "run", "--host=0.0.0.0", "--debug", "--reload" ]