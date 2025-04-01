# mindbox-test
Решение тестового задания
Отказоустойчивость:
Жёсткое распределение по зонам (DoNotSchedule)
PodDisruptionBudget с minAvailable: 3
Graceful shutdown с preStop hook
Экономия ресурсов:
Двойное масштабирование: HPA + CronHPA
Ночной режим с 1-2 репликами
Точные requests/limits
Надёжность:
Раздельные пробы (startup/readiness/liveness)
Стабилизационные окна для HPA
Защита от резкого scale-down
Мониторинг:
Аннотации для Prometheus
Метрики CPU/memory для HPA
Для внешнего доступа раскомментируйте LoadBalancer в Service. Полная конфигурация готова к применению в production-среде.