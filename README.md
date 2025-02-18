# Операционные системы UNIX/Linux (Базовый).

Установка и обновления системы Linux. Основы администрирования.


## Linux
`-` История Linux начинается в 1991 году, когда финский аспирант и программист Линус Торвальдс стал разрабатывать ядро операционной системы для своего компьютера.

`-` Свои наработки он выложил на общедоступном сервере, и это стало ключевым событием в истории Linux. Сначала десятки, потом сотни и тысячи разработчиков поддержали его проект - общими усилиями на свет появилась полноценная операционная система.

`-` Первая официальная версия Linux 1.0 вышла в 1994 году. С самого начала и по сей день Linux распространяется как свободное программное обеспечение с лицензией GPL. Это значит, что исходный код операционной системы может увидеть любой пользователь - и не только увидеть, но и доработать его. Единственное условие - измененный, модифицированный код должен быть также доступен всем и распространяться по лицензии GPL. Это важно, так как дает возможность разработчикам использовать код и в то же время не бояться проблем из-за авторских прав.

`-` Сегодня Linux - самая известная и наиболее используемая операционная система с открытым исходным кодом. Как операционная система, Linux - это программное обеспечение, которое находится под всем другим программным обеспечением на компьютере, получая запросы от этих программ и передавая эти запросы на аппаратное обеспечение компьютера.

## Администрирование

`-` Администрирование - это, если не вдаваться в подробности, поддержка и улучшение работы всего компьютерного и офисного оборудования, периферийных устройств, сетевого подключения и т.д. При администрировании Linux большая часть работы протекает в терминале, поэтому стоит начать с использования базовых утилит.


## Виртуальные машины

`-` Виртуальная машина (VM, ВМ) также, как и физические компьютеры, имеет ЦП, память, диски для хранения файлов и при необходимости может подключаться к Интернету. Отличие лишь в том, что компоненты вашего компьютера (аппаратная часть) материальны, а виртуальные машины существуют только в виде кода.

`-` Проще говоря, это виртуальный компьютер, на который можно устанавливать операционную систему и все сопутствующее программное обеспечение, при этом никаких изменений в Вашей основной операционной системе не будет.

`-` Виртуализация — это процесс создания программной (виртуальной) версии компьютера с выделенными ресурсами ЦП, памяти и хранилища, которые «заимствуются» у физического компьютера. Виртуальная машина — это компьютерный файл (образ), который действует как обычный компьютер.

`-` В свою очередь _VirtualBox_ - это программный продукт виртуализации, т.е. инструмент для создания виртуальных машин.



## Part 1. Установка ОС

#### Установи **Ubuntu 20.04 Server LTS** без графического интерфейса. (Используем программу для виртуализации - VirtualBox)


## Part 2. Создание пользователя

#### Создай пользователя, отличного от пользователя, который создавался при установке. Пользователь должен быть добавлен в группу `adm`.


## Part 3. Настройка сети ОС

#### Задай название машины вида user-1  
#### Установи временную зону, соответствующую твоему текущему местоположению.  
#### Выведи названия сетевых интерфейсов с помощью консольной команды.
 
#### Используя консольную команду получи ip адрес устройства, на котором ты работаешь, от DHCP сервера. 
 
#### Определи и выведи на экран внешний ip-адрес шлюза (ip) и внутренний IP-адрес шлюза, он же ip-адрес по умолчанию (gw). 
##### Задай статичные (заданные вручную, а не полученные от DHCP сервера) настройки ip, gw, dns (используй публичный DNS серверы, например 1.1.1.1 или 8.8.8.8).  
##### Перезагрузи виртуальную машину. Убедись, что статичные сетевые настройки (ip, gw, dns) соответствуют заданным в предыдущем пункте.  


## Part 4. Обновление ОС


##### Обнови системные пакеты до последней на момент выполнения задания версии.  


## Part 5. Использование команды **sudo**

##### Разреши пользователю, созданному в [Part 2](#part-2-создание-пользователя), выполнять команду sudo.


## Part 6. Установка и настройка службы времени

##### Настрой службу автоматической синхронизации времени.  


## Part 7. Установка и использование текстовых редакторов 

##### Установи текстовые редакторы **VIM** (+ любые два по желанию **NANO**, **MCEDIT**, **JOE** и т.д.)  
##### Используя каждый из трех выбранных редакторов, создай файл *test_X.txt*, где X -- название редактора, в котором создан файл. Напиши в нём свой никнейм, закрой файл с сохранением изменений.  


## Part 8. Установка и базовая настройка сервиса **SSHD**


##### Установи службу SSHd.  
##### Добавь автостарт службы при загрузке системы.  
##### Перенастрой службу SSHd на порт 2022.  
##### Используя команду ps, покажи наличие процесса sshd. Для этого к команде нужно подобрать ключи.

##### Перезагрузи систему.


## Part 9. Установка и использование утилит **top**, **htop**


##### Установи и запусти утилиты top и htop.  

 

## Part 10. Использование утилиты **fdisk**


##### Запусти команду fdisk -l.


## Part 11. Использование утилиты **df** 



##### Запусти команду df.  
 

##### Запусти команду df -Th.

## Part 12. Использование утилиты **du**


##### Запусти команду du.
##### Выведи размер папок /home, /var, /var/log (в байтах, в человекочитаемом виде)
##### Выведи размер всего содержимого в /var/log (не общее, а каждого вложенного элемента, используя *)



## Part 13. Установка и использование утилиты **ncdu**

##### Установи утилиту ncdu.
##### Выведи размер папок /home, /var, /var/log.


## Part 14. Работа с системными журналами


##### Открой для просмотра:
##### 1. /var/log/dmesg
##### 2. /var/log/syslog
##### 3. /var/log/auth.log  


## Part 15. Использование планировщика заданий **CRON**

##### Используя планировщик заданий, запусти команду uptime через каждые 2 минуты.

##### Удали все задания из планировщика заданий.
