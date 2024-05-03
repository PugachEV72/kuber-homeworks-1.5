# Домашнее задание к занятию `«Сетевое взаимодействие в K8S. Часть 2»` - Пугач Евгений.


---

## `Задание 1. Создать Deployment приложений backend и frontend`

1. Создать Deployment приложения frontend из образа nginx с количеством реплик 3 шт.
2. Создать Deployment приложения backend из образа multitool.
3. Добавить Service, которые обеспечат доступ к обоим приложениям внутри кластера.
4. Продемонстрировать, что приложения видят друг друга с помощью Service.
5. Предоставить манифесты Deployment и Service в решении, а также скриншоты или вывод команды п.4.


### Ответ:

![Скриншот 1](https://github.com/PugachEV72/Images/blob/master/2024-05-03_23-48-46.png)

![Скриншот 2](https://github.com/PugachEV72/Images/blob/master/2024-05-03_23-58-25.png)

[Ссылка на frontend-deployment.yaml](https://github.com/PugachEV72/kuber-homeworks-1.5/blob/main/frontend-deployment.yaml)

[Ссылка на backend-deployment.yaml](https://github.com/PugachEV72/kuber-homeworks-1.5/blob/main/backend-deployment.yaml)

---

## `Задание 2. Создать Ingress и обеспечить доступ к приложениям снаружи кластера`

1. Включить Ingress-controller в MicroK8S.
2. Создать Ingress, обеспечивающий доступ снаружи по IP-адресу кластера MicroK8S так, чтобы при запросе только  
   по адресу открывался frontend а при добавлении /api - backend.
3. Продемонстрировать доступ с помощью браузера или curl с локального компьютера.
4. Предоставить манифесты и скриншоты или вывод команды п.2.

### Ответ:

![Скриншот 3](https://github.com/PugachEV72/Images/blob/master/2024-05-04_00-12-38.png)

![Скриншот 4](https://github.com/PugachEV72/Images/blob/master/2024-05-04_00-13-58.png)

[Ссылка на my-ingress.yaml](https://github.com/PugachEV72/kuber-homeworks-1.5/blob/main/my-ingress.yaml)

---
