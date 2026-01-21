# CC Lab-2

This repository contains the CC Lab-2 FastAPI + Locust load testing project.

## How to run server

- Install dependencies:
  pip install -r requirements.txt

- Run the FastAPI server:
  uvicorn main:app --reload

## How to run Locust tests

Example command:
locust -f events_locustfile.py --host http://localhost:8000 --headless -u 100 -r 10 --run-time 2m
