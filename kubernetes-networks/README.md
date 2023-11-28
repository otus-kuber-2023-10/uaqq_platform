# uaqq_platform
uaqq Platform repository

# Выполнено ДЗ №3

 - [Х] Основное ДЗ
 - [ ] Задание со *

## В процессе сделано:
 - Добавлены проверки Pod
 - Создан объект типа Deployment для удобства обновления конфигурации пода
 - Создан сервис типа ClusterIP
 - Установлен и проверен в работе LoadBalancer MetalLB
 - Установлен и проверен в работе Ingress

## Как запустить проект:
 - запустить команду `kubectl apply -f metallb-config.yaml`
 - запустить команду `kubectl apply -f nginx-lb.yaml`
 - запустить команду `kubectl apply -f web-deploy.yaml`
 - запустить команду `kubectl apply -f web-ingress.yaml`
 - запустить команду `kubectl apply -f web-svc-cip.yaml`
 - запустить команду `kubectl apply -f web-svc-headless.yaml`
 - запустить команду `kubectl apply -f web-svc-lb.yaml`

## Как проверить работоспособность:
 - Перейти по ссылке `http://<LB_IP>/web/index.html`

## PR checklist:
 - [X] Выставлен label с темой домашнего задания
