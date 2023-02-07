# int20h_test
## Висновки проєкту

Проаналізувавши данні, які нам надали в форматі CSV файлу, ми визначили, що є три головних події, які впливають на рішенні клієнтів щодо відключення преміум підписки


- Chat Conversation Started
- Chat Conversation Opened 
- Transaction Refund

Загалом це може бути пов'язане з помилковим або надмірним списанням коштів з клієнта, що змушує частіше звертатись до чату підтримки і повертати кошти, це спричиняє негативне сприйняття клієнта програми. Ми проводили аналіз використовуючи 7 моделей аналізу даних. 


- desicion_tree
- random_forest
- ada_boost
- xgboost
- logistic_regression
- svc
- k_neighbors


Дані моделі змогли передбачити відмову від преміум підписки з точністю в середньому до 84%. Якщо говорити про вище наведені події, які впливають на відмову від преміум підписки, то такі моделі як:
(далі наводиться приклад моделей та показників у відсотках за впливом на користувача)

- random_forest
  - Chat Conversation Started - 0.247324
  - Transaction Refund - 0.129012
  - Chat Conversation Opened - 0.313174
- xgboost
  - Chat Conversation Started - 0.572377
  - Transaction Refund - 0.085410
  - Chat Conversation Opened - 0.032860
- ada_boost
  - Chat Conversation Started - 0.6
  - Transaction Refund - 0.3
  - Chat Conversation Opened - 0.0

