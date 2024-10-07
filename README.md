# Отчет по тестированию

## 1. Получение карт пользователя в системе Дентал
**URL**: `http://113.30.190.31:8007/api/cards/user_id/`  
**Ожидание**: 200 + JSON  
**Результат**:  
![Получение карт пользователя](https://github.com/user-attachments/assets/1e0c3ef0-8cc3-4e8f-9f05-a4f456c21437)

---

## 2. Получение карт пользователя в системе FreedomPay
**URL**: `http://113.30.190.31:8007/api/cards/get-cards-list-freedompay/`  
**Ожидание**: 200 + JSON  
**Результат**:  
![image](https://github.com/user-attachments/assets/23d04365-8c21-49ec-9d5e-f6a7684c0948)


---

## 3. Привязка карты
**URL**: `http://113.30.190.31:8007/api/cards/add-card/`  
**Ожидание**: 200 + JSON  
**Результат**:  
![image](https://github.com/user-attachments/assets/fc5bab3b-069f-402d-99ea-74fd4da8b2e2)


**Открываем полученную ссылку:**


![image](https://github.com/user-attachments/assets/e3069a9c-6ffe-44a6-9220-0f4edbe0ce66)


**Видим страницу Freedompay для привязи карты**



---

## 4. Получение текущей подписки пользователя
**URL**: `http://113.30.190.31:8007/api/subscribes/user_d/`  
**Ожидание**: 200 + JSON  
**Результат**:  
![image](https://github.com/user-attachments/assets/17c6e18e-a9b3-4fcb-ad13-9998dc42226d)


---

## 5. Проверка email в белом списке
**URL**: `http://113.30.190.31:8007/api/emails/check-email/`  
**Ожидание**: 200 + JSON  
**Результат**:  
![image](https://github.com/user-attachments/assets/6e8d5842-beb0-4fdd-bc9a-6d51c11c100c)

**404 Case**:  
![image](https://github.com/user-attachments/assets/18b0cf37-ad43-4e1c-8bfe-8637bade46f3)


---

## 6. Инициализация подписки пользователя
**URL**: `http://113.30.190.31:8007/api/subscribes/init/`  
**Ожидание**: 200 + JSON  
**Результат**:  
![image](https://github.com/user-attachments/assets/9938eca1-3032-44be-9784-9b7af26152f9)


---

## 7. Смена плана подписки
**URL**: `http://113.30.190.31:8007/api/subscribes/change-plan/`  
**Ожидание**: 200 + JSON  
**Результат**:  
![image](https://github.com/user-attachments/assets/1618854f-3ceb-4f2c-9ecb-e6a909774f4e)

**400 - Last payment date is empty case**:  
![image](https://github.com/user-attachments/assets/2dd314de-e355-46a8-ad23-531eb867df4b)

**404 Case**:  
![image](https://github.com/user-attachments/assets/22eca0ad-80b8-496d-9ba6-12e502e1067a)


---

## 8. Отписка пользователя
**URL**: `http://113.30.190.31:8007/api/subscribes/unsubscribe/user_id/`  
**Ожидание**: 200 + JSON  
**Результат**:  
![image](https://github.com/user-attachments/assets/a3c1b507-0c14-4e7b-b941-0288e7a00ffb)


---

## 9. Получение платежей пользователя
**URL**: `http://113.30.190.31:8007/api/payments/user_id/`  
**Ожидание**: 200 + JSON  
**Результат**:  
![image](https://github.com/user-attachments/assets/c93d6492-6c2d-4ad7-a5e6-1f2850f05ad1)
 
**404 Case**:  
![image](https://github.com/user-attachments/assets/4dba5cb3-e289-4af2-90ae-dcb0ddecaeeb)


---

## 10. Детальная информация о платеже
**URL**: `http://113.30.190.31:8007/api/payments/detail/payment_id/`  
**Ожидание**: 200 + JSON  
**Результат**:  
![image](https://github.com/user-attachments/assets/c742bc22-7d6b-4b6c-8ebc-9226806e2017)


---

## 11. Инициализация платежа
**URL**: `http://113.30.190.31:8007/api/payments/init-payment/`  
**Ожидание**: 200 + JSON  
**Результат**:  
![image](https://github.com/user-attachments/assets/10a71dbd-0307-42ca-8b9e-3e059ba470f7)
  
**Комментарий**: Метод не активирован на стороне FreedomPay. Формирование запроса и парсинг ответа успешны, в ином случае ответ ошибки был бы пуст, и причина не была бы выявлена.

---

## 12. Получение списка всех платежей в системе
**URL**: `http://113.30.190.31:8007/api/payments/`  
**Ожидание**: 200 + JSON  
**Результат**:  
![image](https://github.com/user-attachments/assets/3cdac12a-d6ab-457e-9adf-297052efcaf1)


---

## 13. Добавление FCM токена
**URL**: `http://113.30.190.31:8007/api/notifications/fcm-push-tokens/`  
**Ожидание**: 200 + JSON  
**Результат**:  
![image](https://github.com/user-attachments/assets/082ed8c6-ca99-4d68-a0a1-708f527e2ae1)

