
0. Если нужно вычистить все данные и настройки от старых запусков, можно использовать команду minikube delete

1. Запуск Kubernetes в minikube с активированным metrics-server 
- Запустить Docker Destktop
- Выполнить команду minikube start --addons=metrics-server 

2. Перейти в рабочу директорю (exc2)

3. Задеплоить тестовое приложение в кубернетисе:
- Выполнить команду kubectl apply -f deployment.yaml
- Выполнить команду ubectl apply -f service.yaml

4. Применить манифест  Horizontal Pod Autoscaler:
- Выполнить команду ubectl apply -f hpa.yaml

5. Узнать IP и порт приложения можно командой minikube service --all

5. Запустить инструмент для подачи нагрузки locust:
- Выполнить команду losuct
- Открыть веб интерфейс locust: http://localhost:8089/

6. Открыть дашборд kubernetes:  
- выполнить команду minikube dashboard