# Лабораторная работа 2. Сравнение сервисов Amazon Web Services и Microsoft Azure. Создание единой кросс-провайдерной сервисной модели.

## Цель работы: 
* Получение навыков аналитики и понимания спектра публичных облачных сервисов без привязки к вендору.
* Формирование у студентов комплексного видения Облака.
## Дано: 
1. Данные лабораторной работы 1.
2. Слепок данных биллинга от провайдера после небольшой обработки в виде SQL-параметров. Символ % в начале/конце означает, что перед/после него может стоять любой набор символов.
3. Образец итогового соответствия, что желательно получить в конце. В этом же документе  
## Необходимо: 
1. Импортировать файл .csv в Excel или любую другую программу работы с таблицами. Для Excel делается на вкладке Данные – Из текстового / csv файла – выбрать файл, разделитель – точка с запятой.
2. Распределить потребление сервисов по иерархии, чтобы можно было провести анализ от большего к меньшему (напр. От всех вычислительных ресурсов Compute дойти до конкретного типа использования - Выделенной стойка в датацентре Dedicated host usage). При этом сохранять логическую концепцию, выработанную в Лабораторной работе 1.
3. Сохранить файл и залить в соответствующую папку на Google Drive.

## Алгоритм работы:
Сопоставить входящие данные от провайдера с его же документацией. Написать в соответствие колонкам справа значения 5 колонок слева, которые бы однозначно классифицировали тип сервиса. Для столбцов IT Tower и Service Family значения можно выбрать из образца. В ходе выполнения работы не отходить от принципов классификации, выбранных в Лабораторной работе 1. Например, если сервис Машинного обучения был разбит на Вычислительные мощности и Облачные сервисы, то продолжать его разбивать и в новых данных.
## Выполнение работы:
### Исходная таблица:
![image](https://github.com/user-attachments/assets/8d76245b-cfa7-4b98-b407-4834d28b3406)
Теперь требуется заполнить недостающие столбцы, опираясь на данные Microsoft Azure.
## Результат заполнения:
![image](https://github.com/user-attachments/assets/d04e0cc8-5f04-4e22-a817-290e64452799)
Для заполнения таблицы надо было понять что из себя представляет каждый сервис.

Сервисы:
1. Azure Analysis Services - полностью управляемая платформа как услуга (PaaS), которая предоставляет модели данных корпоративного уровня в облаке.
2. Azure Data Factory - облачный сервис интеграции данных, позволяющий создавать, планировать и управлять процессами извлечения, трансформации и загрузки данных из различных источников.
3. Azure Database - сервис работы с базами данных, предлагет высокодоступные, масштабируемые и безопасные решения для хранения и управления реляционными данными.
4. Azure Redis Cache - сервис кэширования, который хранит часто запрашиваемые данные в оперативной памяти. Он используется для ускорения доступа к данным, уменьшения нагрузки на базы данных и обеспечения масштабируемости приложений за счет эффективного управления кешем.
5. Azure CDN (Content Delivery Network) - глобальная сеть доставки контента, предназначенная для ускорения загрузки веб-сайтов, приложений и видео за счет кэширования контента на серверах, расположенных ближе к пользователям.
6. Azure Batch - сервис, который позволяет запускать и управлять большими параллельными задачами на виртуальных машинах в облаке.
7. Azure Virtual Machines - служба для предоставления виртуальных машин, таких как Linux и Windows.
8. Azure Data Box - система переноса больших объемов данных в облако. Для передачи используется физическое устройство.
9. Azure Key Vault - сервис для безопасного хранения и управления секретами, ключами, сертификатами, паролями.
10. Azure Scheduler - сервис помогает планировать и автоматизировать выполнение задач в облаке, что упрощает управление задачами.
11. Azure Sentinel - сервис информационной безопасности, который находит угрозы и в облаке, и локально и реагирует на них.

## Вывод:
В ходе работы я обзорно познакомился с различными облачными сервисами от Microsoft. Получил понимание многообразия сервисов, которые предоставляет Microsoft.
