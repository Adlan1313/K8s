# K8s


Простой проект для демонстрации навыков DevOps:

- Docker контейнеризация FastAPI приложения (смотри репозиторий докеризация приложения)
- Деплой в Kubernetes (Yandex Cloud)
- Deployment + Service + Health Checks
- LoadBalancer и авто-масштабирование

## Запуск локально

```bash
docker build -t fastapi-demo:latest .
docker run -d -p 8000:8000 fastapi-demo:latest
curl http://localhost:8000/
```
## Деплой в Кубер
```
kubectl apply -f k8s/
kubectl get pods
kubectl get svc
