FROM python:3.9.19-bullseye
WORKDIR /app
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
EXPOSE 5000 8088
ENV REDIS_HOST=redis-service
CMD ["flask", "run", "--host=0.0.0.0", "--port=5000"]