# CHARLES
## Ex_1:
```
Method: GET
EndPoint: /get_method
request URL params:
name: str
age: int

response:
[
"Str",
"Str"
]
```
### Task:
Perform both Rewrite and BreakPoint (you can disable to avoid stopping on each request)
Modify the URL in Charles so that the name you entered in Postman is sent in the request, but the name returned is the one you substituted in Charles.
***

## Ex_2:
```
Method: POST
EndPoint: /user_info_3
request form data:
name: str
age: int
salary: int

response:
{'name': name,
'age': age,
'salary': salary,
'family': {'children': [['Alex', 24], ['Kate', 12]],
'u_salary_1_5_year': salary * 4}}
```
### Task:
Perform both Rewrite and BreakPoint (you can disable to avoid stopping on each request)

Modify the body in Charles so that the salary you entered in Postman is sent in the request, and the number in u_salary_1_5_year is returned as less than the original from the request.
***

## Ex_3:
```
Method: GET
EndPoint: /object_info_1
request URL params:
name: str
age: int
weight: int

response:
{'name': name,
'age': age,
'daily_food': weight * 0.012,
'daily_sleep': weight * 2.5}
``` 

### Task:
Perform both Rewrite and BreakPoint (you can disable to avoid stopping on each request)
Modify the request parameters in Charles so that the response in Postman has a different name, where daily_food > weight from the request, and daily_sleep < weight from the request.
***

## Ex_4:
```
Method: GET
EndPoint: /object_info_3
request URL params:
name: str
age: int
salary: int

response:
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
### Task:
Perform both Rewrite and BreakPoint (you can disable to avoid stopping on each request)
Make Charles manipulate the server to return a 500 status code.
Make Charles manipulate the server to return a 405 status code.
***

## Ex_5:
```
Method: GET
EndPoint: /object_info_4
request URL params:
name: str
age: int
salary: int

response:
{'name': name,
'age': int(age),
'salary': [salary, str(salary * 2), str(salary * 3)]}
```

### Task:
Perform both Rewrite and BreakPoint (you can disable to avoid stopping on each request)
Make Charles manipulate the server to return a 405 error.
Modify the salary in the request.
Modify (salary * 2) in the response.
***

## Ex_6:
```
Method: POST
EndPoint: /user_info_2
request form data:
name: str
age: int
salary: int

response:
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
### Task:
Perform both Rewrite and BreakPoint (you can disable to avoid stopping on each request)
Make Charles modify the response so that qa_salary_after_1.5_year is renamed to qa_salary_after_1.5_month in Postman's response.
Make sure qa_salary_after_3.5_years is less than qa_salary_after_12_months in the response.
***
