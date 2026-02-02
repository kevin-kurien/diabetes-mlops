# Diabetes Prediction Model – FastAPI + Docker + Kubernetes

This project is a Machine Learning application that predicts whether a person is diabetic based on health metrics such as pregnancies, glucose, blood pressure, BMI, and age. The project demonstrates a full MLOps workflow, including training a model, creating a FastAPI API, Dockerizing the application, and deploying it to Kubernetes using kind.

---

## Running the Project

Clone the repository:

```bash
git clone https://github.com/your-username/diabetes-model-demo.git
```

create a virtual environment:
```
python -m venv .mlops
.\.mlops\Scripts\Activate.ps1
```

install requirement.txt:

```
pip install -r requirements.txt
```
Run the FastAPI application locally:
```
uvicorn main:app --reload --host 0.0.0.0 --port 8000
```
Build the Docker image and run the docker container:

```
docker build -t diabetes-model-demo .

docker run -p 8000:8000 diabetes-model-demo
```
The API will be available at http://localhost:8000/docs.
