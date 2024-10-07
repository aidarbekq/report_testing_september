# Отчет по тестированию

http://113.30.190.31:8007/api/cards/user_id/
Получение карт пользователя в нашей системе
ожидание: 200 + json
результат:
![image](https://github.com/user-attachments/assets/1e0c3ef0-8cc3-4e8f-9f05-a4f456c21437)




http://113.30.190.31:8007/api/cards/get-cards-list-freedompay/
Получение карт пользователя в системе freedompay
ожидание: 200 + json
результат:
![[Pasted image 20241007210314.png]]

http://113.30.190.31:8007/api/cards/add-card/
Привязка карты:
ожидание: 200 + json
результат:
![[Pasted image 20241007210126.png]]


http://113.30.190.31:8007/api/subscribes/user_d/
Получение текущей подписки юзера
ожидание: 200 + json
результат:
![[Pasted image 20241007210025.png]]


http://113.30.190.31:8007/api/emails/check-email/
Проверка имейла в вайтлисте
ожидание: 200 + json
результат:
![[Pasted image 20241007211145.png]]
404 case:
![[Pasted image 20241007214658.png]]


http://113.30.190.31:8007/api/subscribes/init/
Инициализация подписки юзера
ожидание: 200 + json
результат:
![[Pasted image 20241007211620.png]]




http://113.30.190.31:8007/api/subscribes/change-plan/
Смена плана юзера в подписке:
ожидание: 200 + json
результат:
![[Pasted image 20241007212430.png]]


400 - last payment date field is empty case: 
![[Pasted image 20241007212132.png]]

404 case:
![[Pasted image 20241007212306.png]]



http://113.30.190.31:8007/api/subscribes/unsubscribe/user_id/
Отписка юзера:
ожидание: 200 + json
результат:
![[Pasted image 20241007212755.png]]



http://113.30.190.31:8007/api/payments/user_id/
Получание платежей юзера
ожидание: 200 + json
результат:
![[Pasted image 20241007213043.png]]

404 case:
![[Pasted image 20241007212945.png]]



http://113.30.190.31:8007/api/payments/detail/payment_id/
Детальное получение определенного платежа
ожидание: 200 + json
результат:
![[Pasted image 20241007213212.png]]



http://113.30.190.31:8007/api/payments/init-payment/
Инициализация платежа
ожидание: 200 + json
результат:
![[Pasted image 20241007213408.png]]
Метод не активирован на стороне фридом
Формирование запроса и парсинг ответа успешны, в ином случае ответ ошибки был бы пуст и причина была бы не выявлена


http://113.30.190.31:8007/api/payments/
Получание списка всех платежей в системе дентал:
ожидание: 200 + json
результат:
![[Pasted image 20241007213520.png]]




http://113.30.190.31:8007/api/notifications/fcm-push-tokens/
Добавление fcm токена:
ожидание: 200 + json
результат:
![[Pasted image 20241007213742.png]]
