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
 - запустить команду `kubectl apply -f frontend-deployment.yaml`
 - запустить команду `kubectl apply -f frontend-replicaset.yaml`
 - запустить команду `kubectl apply -f nodeexporter-daemonset.yaml`, `kubectl port-forward <имя любого pod в DaemonSet> 9100:9100`, `curl localhost:9100/metrics`
 - запустить команду `kubectl apply -f paymentservice-deployment-bg.yaml`
 - запустить команду `kubectl apply -f paymentservice-deployment-reverse.yaml`
 - запустить команду `kubectl apply -f paymentservice-deployment.yaml`
 - запустить команду `kubectl apply -f paymentservice-replicaset.yaml`

## Как проверить работоспособность:
 - Перейти по ссылке `localhost:9100/metrics`

## PR checklist:
 - [X] Выставлен label с темой домашнего задания
