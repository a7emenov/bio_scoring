# Утилита командной строки на языке Scala

1. Инструкция по сборке:  
  1.1. Установить Scala Build Tool (sbt):
    ```
    echo "deb https://dl.bintray.com/sbt/debian /" | sudo tee -a /etc/apt/sources.list.d/sbt.list
    sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 2EE0EA64E40A89B84B2DF73499E82A75642AC823
    sudo apt-get update
    sudo apt-get install sbt
    ```  
    1.2. Запустить команду ```sbt assembly``` в корне проекта. Результатом её работы 


2. Инструкция по запуску:
  Для запуска проекта используется команда ```java -jar <file>```. Предполагается, что на компьютере установлен JDK версии не ниже 8.
  Дополнительные опции запуска:
    ```
    --seq1 <value>           Путь к файлу первой последовательности
    --seq2 <value>           Путь к файлу второй последовательности
    -s, --sequenceType <value>
                             Тип последовательностей (n - нуклеотиды, p - протеины)
    -g, --gap <value>        Штраф за пропуски
    --group <value>          Размер групп, на которые разделяются выровненные последовательности
    --help                   Напечатать вспомогательное сообщение
    ```
  
4. Пример работы алгоритма
