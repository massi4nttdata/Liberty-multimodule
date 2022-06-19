# Liberty multimodule

## Liberty Profile
To install Liberty and Eclipse, you will:

- Set up installation directories

- Install a JDK (jdk-11.0.15.1_windows-x64_bin\jdk-11.0.15.1)

- Install Liberty profile (Open Liberty Version 22.0.0.6 - (22.0.0.6-202205231626))

- Install Eclipse (Version: 2022-03 (4.23.0))

- Install the WebSphere Developer Tools: (Open Liberty Tools for Eclipse, Version: 21.0.0.6,Build id: 2021-06-29_1604)

- Install Liberty Server in Eclipse

follow:
#### https://www.ibm.com/cloud/blog/liberty-and-eclipse-installing-dev-environment-p9

## Maven multimodule
- EAR
 - REST API (war packaging)
 - EJB3 (ejb3.jar)
 - MyBatis (lib/mybatis.jar)
 - h2 database (lib/h2.jar)

## H2 database
download:
#### https://h2database.com/html/download.html
install than:

```bash
C:\Program Files (x86)\H2\bin>java -cp h2-2.1.214.jar org.h2.tools.Shell
Welcome to H2 Shell 2.1.214 (2022-06-13)
Exit with Ctrl+C
[Enter]   jdbc:h2:~/test
URL       jdbc:h2:~/test
[Enter]   org.h2.Driver
Driver
[Enter]
User      sa
Password
Type the same password again to confirm database creation.
Password
Connected
```
http://localhost:8082/



```sql
CREATE TABLE IF NOT EXISTS USERS(ID INT PRIMARY KEY, NAME VARCHAR(255), AGE INT, SURNAME VARCHAR(255));
insert into users(id, name, surname, age) values (50, 'Alice', 'Smith', 45);
```


