## Wednesday 21/10/2019
##### Problem: Jenkins startup
Suggested Solution:
* java -jar jenkins.war --httpPort=8080
* URL: http://localhost:8080/
* ...

*Tags: jenkins*

---
## Monday 20/04/2020
##### Problem: Update TestCafe
Suggested Solution:
* npm outdated (-g for global)
* npm update testcafe (-g for global)
* ...

*Tags: TestCafe*

---
## Wednesday 17/02/2021
##### Problem: SQL Server - Identify most rcently modified stored procedures
Suggested Solution:
```
select name,create_date,modify_date
from sys.procedures
order by modify_date desc
```

*Tags: sql*

---
## Thursday 25/02/2021
##### Problem: Check .NET runtime versions
Suggested Solution:

You can see which versions of the .NET runtime are currently installed with the following command.
```
dotnet --list-runtimes
```

*Tags: .NET*

---
