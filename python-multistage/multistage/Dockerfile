FROM python:3.10-slim AS builder

WORKDIR /app

COPY . .

#### STAGE 2

FROM gcr.io/distroless/python3-debian11

COPY --from=builder /app/main.py /app/main.py

WORKDIR /app

CMD ["main.py"]
