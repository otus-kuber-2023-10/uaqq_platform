# uaqq_platform
uaqq Platform repository

# Выполнено ДЗ №2

 - [Х] Основное ДЗ
 - [Х] Задание со *

## В процессе сделано:
 - Установлена консольная утилита для управления кластерами Kubernetes kubectl.
 - Установлен Minikube.
 - Создан Dockerfile с веб-сервером, отдающим содержимое директории /app.
 - Написан манифест pod `web-pod.yml` для веб-сервера, получены навыки и умения в создании init контейнеров.
 - Написан манифест для запуска frontend части приложения hipstershop.
 - Найдена и исправлена причина, по которой pod frontend приложения hipstershop находится в статусе Error.

## Как запустить проект:
 - запустить команду `kubectl apply -f frontend-pod-healthy.yml`
 - запустить команду `kubectl apply -f web-pod.yml`, а затем команду `kubectl port-forward --address 0.0.0.0 pod/web 8000:80`

## Как проверить работоспособность:
 - Перейти по ссылке http://localhost:8000/homework.html
 - Перейти по ссылке http://localhost:8000/index.html

## PR checklist:
 - [X] Выставлен label с темой домашнего задания
