# Отчёт по  1-му заданию

* Студент: Михеев Богдан
* Для работы я использовал кластер в MongoDB Atlas и GUI MongoDB Compass
* Используемый датасет - Mall Customers Dataset (первый среди предложенных)

1. Датасет загружен через gui Compass, на скриншоте переключение на работу с созданной коллекцией

   ![image](https://user-images.githubusercontent.com/55896560/157307474-a93cf40c-c40b-4be8-803f-7c2b7282ccda.png)

2. Запрос: 3 посетителя, которым по 20 лет

   ![image](https://user-images.githubusercontent.com/55896560/157307687-a762f9b4-8b6f-403c-96c3-57c7d1b8dc56.png)
   
3. Запрос: 3 самые молодые женщины

   ![image](https://user-images.githubusercontent.com/55896560/157307822-9a2c5f2c-b409-428d-b6ef-ff373a87b2f2.png)

4. Запрос: 3 самых старых мужчин

   ![image](https://user-images.githubusercontent.com/55896560/157307931-3f5c9ea9-5c0c-4a9c-82d7-42e6f446c83d.png)

5. Добавим новое поле первому пользователю

   ![image](https://user-images.githubusercontent.com/55896560/157308063-4b012eae-9f82-4179-98f4-7304f0d2df09.png)
   
   Обновление отобразилось в документе:
   
   ![image](https://user-images.githubusercontent.com/55896560/157308090-22137a46-5a36-4e0f-abb9-42b3dcba2fd7.png)

6. Удалим поле дохода у всех мужчин

   ![image](https://user-images.githubusercontent.com/55896560/157308172-332a1c88-d2d9-4aff-b128-5c592a8306eb.png)
   
   Обновление отобразилось в документах:
   
   ![image](https://user-images.githubusercontent.com/55896560/157308206-9520bf56-e69d-4f1b-b242-ea07a677a054.png)

7. Посмотрим на количество просмотренных документов по запросу поиска людей страше 20 и моложе 50 без индексации 
   (оно равно 200, это общее число документов)

   ![image](https://user-images.githubusercontent.com/55896560/157308343-43a4beb0-8d4b-4cae-9fef-53045cf13cfc.png)

8. Проведём индексацию по полю Age

   ![image](https://user-images.githubusercontent.com/55896560/157308458-20ff7fa2-1fe2-447e-939a-be205adcd3fb.png)

9. После индексации по тому же запросу было просмотрено всего 148 документов, что говорит о повышении производительности.

   ![image](https://user-images.githubusercontent.com/55896560/157308549-4af730d9-8f65-4303-a1c6-92007a521a15.png)
   ![image](https://user-images.githubusercontent.com/55896560/157308564-38e92608-7915-427c-b3cc-9ea2d1dbc033.png)
