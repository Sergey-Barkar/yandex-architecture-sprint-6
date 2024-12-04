# Задание 1
## Масштабирование
Использование REST API подразумевает использование stateless компонентов, которые хорошо поддаются горизонтальному масштабированию. Следовательно HPA является оптимальным в данном случае. 
## Отказоустойчивость 
Поскольку недоступность приложения InsureTech имеет периодический характер, ключевым решением данной проблемы является создание специфическим метрик для идентификации проблемы.
Что касается СУБД шаблон PostgeSQL Patroni, представленный в рамках теории к данному модулю, является приемлемым для целей компании по созданию отказоустойчивого решения.
Active-active стратегия позволит лучше распределять нагрузку среди активных пользователей.
## Балансировка нагрузки
Балансировщик нагрузки уже реализован в рамках решения, однако, для улучшения опыта использования продукции компании среди региональных клиентов необходимо наличие геораспределенных ЦОД с GSBL.