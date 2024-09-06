**Основная часть**

Необходимо создать собственные workflow для двух типов задач: bug и остальные типы задач. Задачи типа bug должны проходить жизненный цикл:

1. Open -> On reproduce.

2. On reproduce -> Open, Done reproduce.

3. Done reproduce -> On fix.

4. On fix -> On reproduce, Done fix.

5. Done fix -> On test.

6. On test -> On fix, Done.

7.Done -> Closed, Open.

Остальные задачи должны проходить по упрощённому workflow:

1. Open -> On develop.

2. On develop -> Open, Done develop.

3. Done develop -> On test.

4. On test -> On develop, Done.

5. Done -> Closed, Open.

**Что нужно сделать**

1. Создайте задачу с типом bug, попытайтесь провести его по всему workflow до Done.

2.Создайте задачу с типом epic, к ней привяжите несколько задач с типом task, проведите их по всему workflow до Done.

3.При проведении обеих задач по статусам используйте kanban.

4.Верните задачи в статус Open.

5. Перейдите в Scrum, запланируйте новый спринт, состоящий из задач эпика и одного бага, стартуйте спринт, проведите задачи до состояния Closed. Закройте спринт.

6. Если всё отработалось в рамках ожидания — выгрузите схемы workflow для импорта в XML. Файлы с workflow и скриншоты workflow приложите к решению задания.



**Решение**

Создадим задачу с типом Bug

Создадим кастомный workflow

И создадим Канбан-доску по котору прогоним нашу задачу

![alt text](https://github.com/mezhibo/livecycle-software/blob/6f3ad50b328a9a0a18a91c3905e258b2b4f8ffb6/IMG/1.jpg)


Создадим задачу с типом Other и прогоним ее по упрощенному Workflov

![alt text](https://github.com/mezhibo/livecycle-software/blob/6f3ad50b328a9a0a18a91c3905e258b2b4f8ffb6/IMG/2.jpg)


Теперь создадим Эпик задачу и привяжем к ней 2 простых таски и провезем по всему пути


![alt text](https://github.com/mezhibo/livecycle-software/blob/6f3ad50b328a9a0a18a91c3905e258b2b4f8ffb6/IMG/3.jpg)

Далее создадим Скрам-доску 

![alt text](https://github.com/mezhibo/livecycle-software/blob/6f3ad50b328a9a0a18a91c3905e258b2b4f8ffb6/IMG/4.jpg)

Создадим для нее спринт и прогоним его

![alt text](https://github.com/mezhibo/livecycle-software/blob/6f3ad50b328a9a0a18a91c3905e258b2b4f8ffb6/IMG/5.jpg)


И видим что спринт у нас удачно завершился

![alt text](https://github.com/mezhibo/livecycle-software/blob/6f3ad50b328a9a0a18a91c3905e258b2b4f8ffb6/IMG/6.jpg)


**Теперь выгрузим схемы workflow в xml:**

[BUG](https://github.com/mezhibo/livecycle-software/blob/6f3ad50b328a9a0a18a91c3905e258b2b4f8ffb6/IMG/bug.xml)

[OTHER](https://github.com/mezhibo/livecycle-software/blob/6f3ad50b328a9a0a18a91c3905e258b2b4f8ffb6/IMG/other.xml)



