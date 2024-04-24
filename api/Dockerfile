FROM python:3.9-alpine
WORKDIR /api
COPY main.py api/main.py
COPY requirements.txt api/requirements.txt
RUN pip install -r api/requirements.txt
EXPOSE 8000
CMD ["uvicorn", "api.main:app", "--host", "0.0.0.0", "--port", "8000", "--reload"]
