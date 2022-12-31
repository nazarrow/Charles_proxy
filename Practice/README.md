# Charles proxy. Traffic capture

|Column 1|Column 2|
|:---:|:---:|
|Protocol: |http|
|IP: |162.55.220.72|
|Port: |5005|

***Все настройки Charles выгрузить в GitHub***

*Задание 1. Сделать в Rewrite и в BreakPoint (можно отключить чтобы не стопило на каждом запросе):*
- *Подменить url в Charles чтобы в запросе ушло имя которые вы вписали в Postman, а вернулось то, которое вы подставили в Charles.* 

Postman:

Request:

```
Method: GET  
EndPoint: /get_method  
Url params:  
name: str  
age: int  
```

Response: 

```json
[
    “Str”,
    “Str”
]
```

## [[Link] Task 1 completion](https://drive.google.com/file/d/1uAcVEPFuZqJsQlKI-vhOIsKQA0QacXVz/view?usp=share_link)

---

*Задание 2. Сделать в Rewrite и в BreakPoint (можно отключить чтобы не стопило на каждом запросе):*
- *Подменить body в Charles так чтобы в запросе ушла salary которую вы вписали в Postman, а в u_salary_1_5_year цифра вернулась меньше оригинальной из запроса.*

Postman:

Request:

```
Method: POST
EndPoint: /user_info_3
Body/form data: 
name: str
age: int
salary: int
```

Response: 

```json
{'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'u_salary_1_5_year': salary * 4}}

```

## [[Link] Task 2 completion](https://drive.google.com/file/d/195j2DgqBnd2ywhX5lZc8kQj4oQrXHRaP/view?usp=share_link)

---

*Задание 3. Сделать в Rewrite и в BreakPoint (можно отключить чтобы не стопило на каждом запросе):*
- *Подменить параметры запроса в Charles так, чтобы в Postman пришел ответ где другое name, daily_food > weight из запроса, а daily_sleep < weight из запроса.*

Postman:

Request:

```
Method: GET
EndPoint: /object_info_1
Url params: 
name: str
age: int
weight: int
```

Response: 

```json
{'name': name,
          'age': age,
          'daily_food': weight * 0.012,
          'daily_sleep': weight * 2.5}
```

## [[Link] Task 3 completion](https://drive.google.com/file/d/1jD4UhYEMHWC1CIsLiv1x2bDjzqTWlx_2/view?usp=share_link)

---

*Задание 4. Сделать в Rewrite и в BreakPoint (можно отключить чтобы не стопило на каждом запросе):*
- *Сделать через Charles так, чтобы сервер вернул 500 код;*
- *Сделать через Charles так, чтобы сервер вернул 405 код.*
  
Postman:

Request:

```
Method: GET
EndPoint: /object_info_3
Url params: 
name: str
age: int
salary: int
```

Response: 

```json
{'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'pets': {'cat':{'name':'Sunny',
                                     'age': 3},
                              'dog':{'name':'Luky',
                                     'age': 4}},
                     'u_salary_1_5_year': salary * 4}
          }
```

## [[Link] Task 4 completion](https://drive.google.com/file/d/1K2jqlnEjysqYo8BgC8WTL3vwh6w_dZv4/view?usp=share_link)

---

*Задание 5. Сделать в Rewrite и в BreakPoint (можно отключить чтобы не стопило на каждом запросе):*
- *Сделать через Charles так, чтобы сервер вернул 405 ошибку;*
- *Подменить salary в request;*
- *Подменить (salary * 2) в response.* 

Postman:

Request:

```
Method: GET
EndPoint: /object_info_4
Url params: 
name: str
age: int
salary: int
```

Response: 

```json
{'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }
```

## [[Link] Task 5 completion](https://drive.google.com/file/d/1pQNMa9sHL1G__WBto0UkxWulJyHte_wi/view?usp=share_link)

---

*Задание 6. Сделать в Rewrite и в BreakPoint (можно отключить чтобы не стопило на каждом запросе):*
- *Сделать через Charles так, чтобы в Postman вернулся ответ, в котором qa_salary_after_1.5_year переименовано в qa_salary_after_1.5_month;*
- *Сделать так чтобы qa_salary_after_3.5_years было меньше qa_salary_after_12_months в response.*

Request:

```
Method: POST
EndPoint: /user_info_2
Body/form data: 
name: str
age: int
salary: int
```

Response: 

```json
{'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }
```

## [[Link] Task 6 completion](https://drive.google.com/file/d/1STMVMiATHBhUGh_9SLRr5vCx5PkLLLSk/view?usp=share_link)

---


