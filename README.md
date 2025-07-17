# k8s-deploy-app - Kubernetes

Команда:

`minikube ssh`

подключает к виртуальной машине (VM), внутри которой работает Kubernetes кластер, созданный через Minikube.

---

Команда:

`kubectl apply -f deployment.yaml`

используется в Kubernetes для применения конфигураций из YAML-файла. Она создаёт или обновляет объекты (Deployment, Service, ConfigMap и т.д.) в кластере на основе содержимого указанного файла.

--- 

Команда:

`kubectl get deploy`

отображает список всех Deployment в текущем namespace Kubernetes.

---

Команда:

`kubectl get svc`

выводит список всех Kubernetes сервисов (Services) в текущем namespace.

---

Команда:

`kubectl get pods`

показывает список всех Pod'ов в текущем namespace Kubernetes.

---

Команда:

`kubectl describe pod <pod-name>`

выводит подробную информацию о Pod'е, включая:
- события (Events)
- статус контейнеров
- volume'ы
- переменные окружения
- ресурсы
- причины ошибок (CrashLoopBackOff, ImagePullBackOff, и т.д.)