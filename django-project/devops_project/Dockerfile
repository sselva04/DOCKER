FROM ubuntu

WORKDIR /app

COPY requirements.txt /app
COPY devops_project /app

RUN apt-get update && \
    apt-get install -u python3 python3-pip && \
    pip install -r requirements.txt && \
    cd devops_project

ENTRYPOINT ["python3"]
CMD ["manage.py", "runserver","0.0.0.0:8000"]