FROM python:3.9-slim

WORKDIR /app 

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

ENV FLASK_APP=token_validation

EXPOSE 5001

# CMD [ "flask", "run", "--host=0.0.0.0" ]

CMD [ "python3", "token_validation.py" ]