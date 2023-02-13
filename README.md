"# counter-api" -------http://localhost:2020/swagger-ui/index.html#/
Write a simple rest-based java application, with a simple frontend of your choice, that can do the following:

1. Create new Counter(s)
2. Increment a named counter by 1
3. Get a current value of a counter
4. Get a list of all counters and their current values

How to execute the application
1)clone the repo
2)use any  IDD(eclipse  or Intellij ) to import or open the maven project
3)run- mvn clean (on terminal or through IDE)
5)mvn install
6)run as java application -CounterApiApplication.java 
 
7)To access swagger url

http://localhost:2020/swagger-ui/index.html#/

Below are 4 rest Apis

​i)
GET-/counter​/{counterName}

Request URL
http://localhost:2020/counter/Priyanka

Response body

{
  "counterName": "Priyanka",
  "counterCount": 3
}

ii)
GET-/counter​/counters
Request URL
http://localhost:2020/counter/counters
Response body

[
  {
    "counterName": "counter2",
    "counterCount": 1
  },
  {
    "counterName": "counter3",
    "counterCount": 2
  },
  {
    "counterName": "counter4",
    "counterCount": 2
  },

  {
    "counterName": "string",
    "counterCount": 1
  },
  {
    "counterName": "counter1",
    "counterCount": 3
  },
  {
    "counterName": "Priyanka 2 counter",
    "counterCount": 2
  },
  {
    "counterName": "Priyanka",
    "counterCount": 3
  }
]
iii)
POST-/counter​/create

Request URL
http://localhost:2020/counter/create
	
Response body

Request URL
http://localhost:2020/counter/create

Request Body

{
"counterName": "Counter100"
}
	
Response body

{
  "counterName": "Counter100",
  "counterCount": 1
}
iv)
​PUT/counter​/increment
Request URL
http://localhost:2020/counter/increment
Request Body

{
"counterName": "Counter100"
}
	
	
Response body

{
  "counterName": "Counter100",
  "counterCount": 2
}


Note: if application is ran multiple times(more than 3-4 times) from same system and db connection issue comes. Pls restart the system.