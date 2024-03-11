1) Установил и запустил monga
![](/dbm_1_hw_screens/install1.png)
![](/dbm_1_hw_screens/install2.png)

2) Создал базу данных и коллекцию в ней
![](/dbm_1_hw_screens/create_col.png)

3) Загрузил данные, проверил что все сохранилось как надо. После загрузки датасета переделал скачанный .data в .csv, но в принципе можно было передавать и .data + список имен колонок еще одним аргументом.
![](/dbm_1_hw_screens/load_data.png)

4) CRUD запросы
![insert](/dbm_1_hw_screens/insert.png)
![find](/dbm_1_hw_screens/find.png)
![update](/dbm_1_hw_screens/update.png)
![delete](/dbm_1_hw_screens/delete.png)

5) Создал индекс
![](/dbm_1_hw_screens/create_idx.png)

6) Сравнил производительность для операции на проиндексированной колонке и непроиндексированной. В силу малого размера датасета различия по времени не было, однако в executionStats параметры totalDocsExamined различаются - в случае наличия индекса проверялось в разы меньше записей, а значит при большом размере коллекции работало бы быстрее.
![с индексом](/dbm_1_hw_screens/report_idx.png)
![без индекса](/dbm_1_hw_screens/report_no_idx.png)
