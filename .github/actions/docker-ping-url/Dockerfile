# Stage 1: Build stage
FROM python:alpine3.23

WORKDIR /app

# Install build dependencies

COPY requirements.txt .

RUN python3 -V
RUN pip install --no-cache-dir -r requirements.txt

#Copy wvwrything into current directrory
#COPY --from=builder /install /usr/local
COPY . .




WORKDIR /app


CMD [ "python", "/app/main.py" ]