# k8s-deploy-app - Kubernetes

Команда:

`docker exec -it <container-name> sh`

— используется для входа внутрь работающего Docker-контейнера и запуска в нём интерактивной оболочки sh.

Что делает каждый параметр:
docker exec — запускает команду внутри уже запущенного контейнера.

- -i — запускает команду в интерактивном режиме (stdin открыт).
- -t — выделяет терминал (TTY), чтобы можно было взаимодействовать через консоль.
- <container-name> — имя или ID контейнера, куда хочешь зайти.
- sh — запускает простую команду оболочки (shell).

---

Команда:

`docker ps`

показывает список всех запущенных контейнеров на текущем clustere

---

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