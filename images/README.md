# Домашнее задание к занятию 12.6 «Репликация и масштабирование. Часть 1» Баранов Сергей


---


### Задание 1

На лекции рассматривались режимы репликации master-slave, master-master, опишите их различия.

*Ответить в свободной форме.*

Различие конфигураций предполагает назначение дополнительных серверов в схеме, репликация master-master позволяет копировать данные с одного сервера на другой. Эта конфигурация добавляет избыточность и повышает эффективность при обращении к данным. 
Master-slave конфигурация преподлагает наличие главной ноды, куда поступают все операции с данными, а далее на слейв-ноды эта информация распостраняется для надежности и позволяет оттуда читать данные,снижая нагрузку на мастер-ноду
master-slave - используется один master сервер где записываются все изменения данных и один или несколько серверов slave с которых происходит чтение данных master-master - сервера в точности повторяющие друг-друга и одновременно, выступающие в роли slave и master, данные сохраняются на всех master серверах


---


### Задание 2

### Выполните конфигурацию master-slave репликации, примером можно пользоваться из лекции.

*Приложите скриншоты конфигурации, выполнения работы: состояния и режимы работы серверов.*

![monitoring](https://github.com/12sergey12/12.6_Replication/blob/main/images/12.6-2.png)

![monitoring](https://github.com/12sergey12/12.6_Replication/blob/main/images/12.6-2sl.png)

![monitoring](https://github.com/12sergey12/12.6_Replication/blob/main/images/12.6-2conf_m.png)

![monitoring](https://github.com/12sergey12/12.6_Replication/blob/main/images/12.6-2conf_sl.png)

![monitoring](https://github.com/12sergey12/12.6_Replication/blob/main/images/12.6-2pos_m.png)

![monitoring](https://github.com/12sergey12/12.6_Replication/blob/main/images/12.6-2repl_sl.png)

![monitoring](https://github.com/12sergey12/12.6_Replication/blob/main/images/12.6-2st_sl.png)

![monitoring](https://github.com/12sergey12/12.6_Replication/blob/main/images/12.6-2st_sl_.png)

---

