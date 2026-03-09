# Python Docker Test

A very simple Python application containerized with Docker.
This project was created for learning and practicing Docker basics such as building images, running containers, and pushing images to Docker Hub.

## 📌 Project Structure

```
python-docker-test
│
├── app.py
└── Dockerfile
```

## 🐍 Python Code

`app.py`

```python
print("Hello from Docker Python App 🚀")
```

This script simply prints a message when the container runs.

## 🐳 Dockerfile

```
FROM python:3.10-slim

WORKDIR /app

COPY app.py .

CMD ["python", "app.py"]
```

### Explanation

* **FROM** – Uses the official Python base image.
* **WORKDIR** – Sets the working directory inside the container.
* **COPY** – Copies the Python file into the container.
* **CMD** – Runs the Python script when the container starts.

## ⚙️ Build the Docker Image

Run the following command in the project directory:

```
docker build -t cardosomatine/python-test .
```

## ▶️ Run the Container

```
docker run cardosomatine/python-test
```

Expected output:

```
Hello from Docker Python App 🚀
```

## ☁️ Docker Hub Image

The image is available on Docker Hub:

```
docker run cardosomatine/python-test
```

## 🎯 Purpose of This Project

This project was created to practice:

* Docker basics
* Creating Docker images
* Running containers
* Pushing images to Docker Hub

## 🚀 Future Improvements

Possible next steps:

* Build a Python API with Flask
* Use Docker Compose
* Connect to a database (MySQL or PostgreSQL)
* Containerize a Django application

## 👨‍💻 Author

Created by **Cardoso Matine** as part of learning backend development and containerization.
