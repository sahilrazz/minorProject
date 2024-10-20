# frontent/Dockerfile

FROM python:3.8-slim-buster

COPY requirements.txt app/requirements.txt

WORKDIR /app

RUN pip install -r requirements.txt
# RUN pip install altair

COPY . /app

EXPOSE 8501

ENTRYPOINT ["streamlit","run"]
CMD ["app.py"]