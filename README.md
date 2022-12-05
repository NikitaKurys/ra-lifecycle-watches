# ra-lifecycle-watches
Мировые часы
Мировые часы
===

Наверняка вы видели в офисах многих компаний, установленные часы, показывающие время в разных столицах мира:
* New York
* Moscow
* London
* Tokyo 

И т.д.

![Watches](https://github.com/netology-code/ra16-homeworks/raw/master/lifecycle-http/watches/assets/watches.png)

Общая механика:

1. Вы заполняете поля название и временная зона (указываете смещение в часах относительно Гринвича) и нажимаете кнопку "Добавить"
1. Часы автоматически добавляются и (что самое важное) часы начинают "тикать", т.е. отсчитываются секунды, минуты и часы
1. При нажатии на крестик рядом с часами часы автоматически удаляются, при этом все подписки (`setTimeout`, `setInterval` и другие) должны вычищаться в соответствующем методе жизненного цикла

Упрощения: если вам сложно реализовать механику со стрелками (через css - см. `transform` и `rotate()`), то вы можете сделать цифровые часы, где отображаются только цифры в формате: ЧЧ:ММ:СС

Подсказки:
1. Посмотреть текущий TimezoneOffset вы можете используя объект `Date`
1. Можете использовать библиотеку momentjs.

---


[![Build status](https://ci.appveyor.com/api/projects/status/6lx029k67uds3xkm/branch/main?svg=true)](https://ci.appveyor.com/project/NikitaKurys62983/ra-lifecycle-watches/branch/main)