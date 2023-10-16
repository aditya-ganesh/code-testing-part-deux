FROM python:3.11-slim

RUN pip install --no-cache-dir --upgrade pip && \
    pip install --no-cache-dir streamlit
RUN mkdir /app

WORKDIR /app
COPY web.py /app/web.py
EXPOSE 8501

ENTRYPOINT ["streamlit","run","web.py"]
