FROM python:3.8
LABEL maintainer="tintd2"

COPY ./techtrends /app
WORKDIR /app
RUN pip install -r requirements.txt
RUN python3 init_db.py

EXPOSE 3111

# command to run on container start
CMD [ "python", "app.py" ]