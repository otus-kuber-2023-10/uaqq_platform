# uaqq_platform
uaqq Platform repository

# Выполнено ДЗ №3

 - [Х] Основное ДЗ
 - [Х] Задание со *

## В процессе сделано:
 - Установлен kind и создан кластер, состоящий из одной мастер ноды и трех воркер нод.
 - Написан `replicaset` для разворачивания трех реплик сервиса frontend.
 - Написан `deployment` для разворачивания трех реплик сервиса frontend.
 - Получены навыки и умения в обновлении версии приложения при помощи deployment с использованием параметров `maxSurge` и `maxUnavailable`, получено понимание в работе стратегий `blue green` и `rolling update`.
 - Получены навыки, умения и понимание работы `Probes`.
 - Получены навыки, умения и понимание работы `Daemonset`.
 - Написан `Daemonset` для Prometheus `NodeExporter`.

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
